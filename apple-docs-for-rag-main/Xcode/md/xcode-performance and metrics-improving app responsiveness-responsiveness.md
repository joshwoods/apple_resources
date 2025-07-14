

- Xcode
- Performance and metrics
-  Improving app responsiveness 

Article

# Improving app responsiveness

Create a user experience that feels responsive by removing hangs and hitches from your app.

## Overview

An app that responds instantly to users’ interactions gives an impression of supporting their workflow. When the app responds to gestures and taps in real time, it creates an experience for users that they’re directly manipulating the objects on the screen. Apps with a noticeable delay in user interaction (a *hang*) or movement on screen that appears to jump (a *hitch*), shatter that illusion. This leaves the user wondering whether the app is working correctly. To avoid hangs and hitches, keep the following rough thresholds in mind as you develop and test your app.

\Understanding user interface responsiveness.

This article describes several best practices to help you avoid introducing hangs and hitches in your app, as well as multiple tools to help you detect and analyze these types of responsiveness issues.

### Avoid hangs by keeping the main thread free from non-UI work

Make sure your app uses the main thread only to interact with the user interface (UIKit, AppKit, or SwiftUI). Direct all other operations to a background thread, operation queue, or Grand Central Dispatch queue. To learn more about hangs and why it’s essential to keep the main thread free from non-UI work, see Understanding hangs in your app.

With Swift concurrency, make sure not to accidentally execute work on the MainActor. The correct approach to get work off of the main actor depends on whether you can refactor the heavy work into a non-actor-isolated asynchronous function. If you can wrap the long-running work in such a way to make it `async` and `nonisolated`, it’s easy to execute it off of the main actor with a `Task` and `await`. If this isn’t possible, execute the synchronous function inside a call to the detached(priority:operation:) function.

Below there are three almost identical code examples. The first one shows how to correctly get off of the main actor if you can wrap the long-running work in a `nonisolated` `async` function. The second example shows a common mistake where the code looks as if it avoids the hang, but doesn’t. This example just causes a hang a little later due to a `Task` implicitly inheriting the actor-constraint from its surrounding context. The last example shows how to break this implicit actor-constraint inheritance by using a detached `Task` instead. The subtle differences in these examples cause completely different execution behavior. Be aware of these in your own Swift concurrency code.

The following code example shows how to successfully get your long-running work off of the main actor if the long-running function is `async` and `nonisolated`, or if you can wrap it in such a function:

```
import SwiftUI

struct ContentView: View {
    var body: some View {
        Button("I don't hang") {
            Task { 
                await doLongRunningWork()
                updateUI()
            }
        }
    }
    @MainActor func updateUI() { /* ... */ }
}
private func doLongRunningWork() async { /* a lot of work */ } // Implicitly nonisolated due to being a free function
```

Creating a `Task` in the above example allows the button action to return immediately, before the new task finishes executing. Specifically, the `Task` itself inherits the actor from its enclosing context and *does* execute on the main actor. Beginning with Swift 5.7, Swift executes nonisolated, asynchronous functions, like `doLongRunningWork()` in the example above, on the concurrency thread pool, off of any actors. Then execution of the `updateUI()` function returns to the main actor because it’s part of a `Task` constrained to the main actor. This is exactly what we want to happen.

Note

For more information about how actors and tasks interact, and the circumstances under which isolated/nonisolated, synchronous/asynchronous functions execute on and off of an actor, see Eliminate data races using Swift concurrency.

Both the `nonisolated` aspect of the function and the `async` nature of it are essential for enabling this behavior. When the long-running work only executes synchronously, it is *not enough* to wrap it in a `Task`. For example, the following code produces a hang:

```
// This code produces a hang. This is only for illustration purposes.
import SwiftUI

struct ContentView: View {
    var body: some View {
        Button("Hang later!") {
            // Don't do this. Use Task.detached {} instead or make `doLongRunningWork()` async.
            Task {
                doLongRunningWork()
                updateUI()
            }
        }
    }
}
private func doLongRunningWork() { /* a lot of work */ } // Nonisolated, but synchronous.
```

Note that this is almost the exact code as in the previous example, except that `doLongRunningWork()` isn’t `async`, so there isn’t an `await` keyword before the function call. This *does* create a separate Swift concurrency task and allows the button’s action to return quickly without blocking the UI. However, the created task inherits the context from its enclosing context because the `body` property on the SwiftUI `View` is annotated with `@MainActor`, meaning it must execute on the main actor.

By default, tasks inherit their context from their enclosing context during creation. Therefore, the newly created task in the `body` property’s context is also constrained to the main actor, which means it can only execute on the main actor and does still block the main actor for a long amount of time. This just *delays* the hang until after the immediate button action finishes. Swift concurrency enqueues the task on the main actor and executes it there shortly after, which keeps the main thread busy and prevents it from handling incoming events.

If making the function `async` isn’t an option, wrap it in a `detached` task to explicitly opt out from inheriting the surrounding execution context.

```
import SwiftUI

struct ContentView: View {
    var body: some View {
        Button("Hang in UI interaction") {
            Task.detached {
                doLongRunningWork()
                await updateUI()
            }
        }
    }
}
private func doLongRunningWork() { /* a lot of work */ } // Nonisolated, but synchronous.
```

This is also often appropriate for background work that can execute at a lower priority and doesn’t need to update the UI when it finishes. Choosing a detached task ensures that the task doesn’t inherit the actor context, so it can execute on any thread in the thread pool. Another difference from the previous example is that the entire task executes outside of the main actor, instead of just the one `async` function. Also note that the code calls `updateUI()` using the `await` keyword because the detached task doesn’t execute on the main actor, so main-actor-constrained functions must execute asynchronously.

Be aware of the default priority propagation rules. A detached task doesn’t inherit any priority from its creation context and executes only with `.medium` priority, by default. Consider choosing a more appropriate priority using `.detached(priority: .background)` or a similar quality-of-service level.

Note

See Visualize and optimize Swift concurrency to learn how to use Instruments to detect when your Swift concurrency tasks execute on the main actor.

When using dispatch queues or manual thread management, dispatch the work to a background queue or thread asynchronously, and have it asynchronously signal the main thread or queue to update the UI when its background work finishes. Don’t synchronize the main thread with a background thread, or make the main thread join a background thread. Both of these actions block the main thread until the work in the background completes, which denies your app the benefit of concurrent operation.

### Analyze which parts of your app need to execute on the main thread and which don’t

Generally, separate your UI updates into preparing data for display, and updating view objects to display that data when the view redraws. Your app can do the preparation in the background, and only needs to use the main thread to update its views. Indicate to the user that this preparation is underway, giving them the opportunity to cancel or perform other tasks as appropriate.

For example, a particular app uses a UIRefreshControl to allow the user to pull a table view down to refresh its content from the network. The `valueChanged` event on the `UIRefreshControl` triggers an action method on the app’s `UIViewController` subclass. When UIKit invokes this action method, the app makes a request to the server using URLSession and `NSURLDataTask`. On completion of the network task, the app checks whether the download succeeds. If it does, the app deserializes a JSON object from the downloaded data, updates properties on its model objects based on the fields in the JSON object, and reconfigures its view to reflect the updated model.

Of all of these tasks, only the action method invocation from UIKit and the reconfiguration of the app’s views need to use the main thread. The app can dispatch all other tasks asynchronously to the background, as the image below shows:

### Use high-level concurrency constructs to avoid having too many threads

As the number of threads running on the device increases, the operating system schedules each thread less often on a CPU core. Any individual thread, including your app’s main thread, runs on a core for less time. So, it’s important to avoid creating too many threads to keep the system performant.

Swift concurrency, Dispatch, and OperationQueue all maintain an internal pool of worker threads that’s tuned to the device capacity and load. Use these technologies, instead of creating your own background threads, to ensure balance between scheduling as much work as possible and allowing the operating system to run other threads, including the main thread and operating system tasks.

### Avoid hitches by minimizing view update time

To provide smooth animations that look like continual motion, Apple devices update the screen up to 120 times per second. When your app is in the foreground, the drawing code on the main thread needs to complete before the next frame is needed to avoid dropping frames and appearing jerky. Taking a long time to draw a frame can cause a hitch.

Use standard views wherever possible to ensure efficient view drawing. Where you need a custom view or control to provide functionality unavailable from standard components, ensure that its draw(_:) method draws only into the specified rectangle. Rely on previously prepared data in `draw(_:)`, don’t perform I/O or complex calculations in this method. Draw only into the rectangle that passes as an argument to `draw(_:)` to avoid expensive computations on view components that don’t draw to the screen.

UIKit and AppKit only invoke a view’s `draw(_:)` method to update the view for a frame if there’s a call to its setNeedsDisplay() method after the most recent call to `draw(_:)`. Only call `setNeedsDisplay()` when the view’s representation needs updating.

To learn more about different types of hitches and the stages of the render loop, see Understanding hitches in your app.

### Optimize your app for variable refresh rates

If your app interacts with the graphics system directly, such as when you do your own rendering, be aware of variable refresh rate displays. If you’re only using high-level UI APIs like SwiftUI, UIKit, and AppKit, those frameworks take care of adapting animations, and similar rendering work, to the display’s refresh rate. If you can’t ensure that the work necessary to prepare the next frame completes within ~5 ms, or your app can adapt its rendering performance and detail based on system conditions, consider adapting your app for variable refresh rates.

In general, it’s better to aim for a slightly lower refresh rate that your app can consistently achieve than attempt to meet a higher refresh rate that sometimes misses the frame deadline, because each missed deadline results in a hitch. Use CADisplayLink or CVDisplayLink to ensure you maximize the time for rendering by starting work on the next frame right when a vsync occurs instead of potentially starting in the middle of a vsync interval.

Note

- See Optimizing ProMotion refresh rates for iPhone 13 Pro and iPad Pro to learn more about working with variable refresh rates.

- See Optimize for variable refresh rate displays to learn about the difference between fixed-rate and adaptive-sync displays, and how to make the most of variable refresh rate displays.

### Write performance tests to ensure main-thread-bound code completes fast

For code that must execute on the main thread, create an XCTest performance test to measure the time your app spends running the code. Execute the relevant code in a measure(_:) block. You can either accept the average runtime of your code block as the baseline, or edit the baseline and set it to 100 ms. The performance test fails if the code requires significantly longer than the baseline time to execute.

100 ms is the maximum delay for discrete user interaction before a delay becomes noticeable. However, be aware that some users are more sensitive to delays, so consider using a lower threshold. Also, remember that code the system runs during continuous user interaction, like table and collection view data source methods, must finish much more quickly. Consider using a limit of 5 ms for such code.

Note

See Eliminate animation hitches with XCTest to learn how to use the XCTOSSignpostMetric to write performance tests measuring the hitch ratio, number of hitches, and similar metrics for a piece of code.

### Detect hangs and hang risks

There are various tools you can use to detect hangs proactively during development, both when you implement a new feature or make a change to an existing part of your app. These tools are also useful to track down a reported issue for a released version of your app.

- Turn on the Thread Performance Checker in your app’s scheme to receive notifications of priority inversions when you run your app from Xcode. Learn more at Diagnosing performance issues early.

- Enable on-device hang detection by opening the Settings app and navigating to Developer \> Hang Detection. This notifies you of hangs that occur in apps on your device while you’re using it. Your iOS device captures a hang report that you can then analyze on your Mac. On-device hang detection works for development-signed builds and TestFlight builds on your iOS device.

- Use the Time Profiler, CPU Profiler, or Hitches templates in Instruments to profile your app proactively. All these templates include the Hangs instruments, which displays any hangs it encounters during the recording and allows you to analyze them further. Hang detection in Instruments was introduced in Instruments 14, and requires macOS 13, iOS 16, tvOS 16, or watchOS 9, or later.

### Find the cause of a hang

Apps hang because the main thread isn’t available when it’s time for the app to react to an event that requires a screen update. This can happen for two reasons: either the main thread is busy executing code, or it’s blocked waiting for a resource to become available or for a system call to complete.

After you detect a specific hang with one of the tools above and can reproduce it, attach your device to your Mac and profile your app with Instruments while reproducing the issue. You can then add additional instruments to your trace document to track down the issue and precisely analyze what causes your hang. You can also import the tailspin files from on-device hang detection into Instruments and perform the same kind of analysis. To learn how to use Instruments to track down and fix hangs, see Getting started with hang analysis, or watch Analyze hangs with Instruments.

### Detect and analyze hitches using Instruments

To proactively look for hitches, or to investigate a specific hitch you’re trying to fix, use the Animation Hitches template in Instruments. Start Instruments, select your app and the Animation Hitches template, and click the Record button. Then use the feature in your app that you want to investigate, and Instruments highlights any hitches that occur.

Get into a habit of profiling your code using the Animation Hitches template whenever you make a change that may affect scrolling or animation behavior. Just a few milliseconds of delay can cause a hitch, so small performance differences can have a big impact. To make sure you get realistic measurements, it’s best to run your app on a real device when looking for hitches with Instruments. Also, consider using older devices that your app supports to make it easier to find issues.

To learn more about how to analyze and fix different types of hitches using Instruments, see Find and fix hitches in the commit phase and Demystify and eliminate hitches in the render phase. To better understand the individual aspects of the render loop the Hitches instrument exposes, see Understand the display refresh interval and associated deadlines.

### Get reports and metrics from the field

Prerelease testing doesn’t always capture all possible issues a user may encounter. In some cases, hangs and hitches in your app escape prerelease testing and make it into the released app. Xcode Organizer bridges the gap between prerelease and postrelease by providing diagnostics for issues users are most frequently experiencing when using your app.

To get a better understanding of how your released app performs, and how many hangs and hitches your users experience, view aggregated data in Xcode Organizer or collect reports using your own infrastructure and MetricKit.

The operating systems on Apple devices monitor for hangs and hitches for running apps, and employ population subsampling to periodically collect reports for these issues. For more information about analyzing the hangs and hitches your users are experiencing, see Analyzing responsiveness issues in your shipping app.

## See Also

### Related Documentation

Analyzing the performance of your shipping app

View power and performance metrics for apps you distribute through the App Store.

Getting started with hang analysis

Learn how to analyze hangs with Instruments.

Analyze hangs with Instruments

Track down hangs with Xcode and on-device detection

Explore UI animation hitches and the render loop

Find and fix hitches in the commit phase

Demystify and eliminate hitches in the render phase

Eliminate animation hitches with XCTest

### Responsiveness

Analyzing responsiveness issues in your shipping app

Identify responsiveness issues your users encounter, and use the hang and hitch data in Xcode Organizer to determine which issues are most important to fix.

Understanding user interface responsiveness

Make your app more responsive by examining the event-handling and rendering loop.

Understanding hangs in your app

Determine the cause for delays in user interactions by examining the main thread and the main run loop.

Understanding hitches in your app

Determine the cause of interruptions in motion by examining the render loop.

Diagnosing performance issues early

Diagnose potential performance issues in your app during testing with the Thread Performance Checker tool in Xcode.

Reducing your app’s launch time

Create a more responsive experience with your app by minimizing time spent in startup.

Reducing terminations in your app

Minimize how frequently the system stops your app by addressing common termination reasons.

Reducing disk writes

Improve your app’s responsiveness by optimizing how it writes data to permanent storage.

