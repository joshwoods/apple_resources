

- UIKit
- UIApplication
-  beginBackgroundTask(withName:expirationHandler:) 

Instance Method

# beginBackgroundTask(withName:expirationHandler:)

Marks the start of a task with a custom name that should continue if the app enters the background.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

**tvOS**

``` source
nonisolated
func beginBackgroundTask(
    withName taskName: String?,
    expirationHandler handler: (@MainActor () -> Void)? = nil
) -> UIBackgroundTaskIdentifier
```

**iOS, iPadOS, Mac Catalyst, visionOS**

``` source
nonisolated
func beginBackgroundTask(
    withName taskName: String?,
    expirationHandler handler: (() -> Void)? = nil
) -> UIBackgroundTaskIdentifier
```

## Parameters 

`taskName`  

The name to display in the debugger when viewing the background task. If you specify `nil` for this parameter, the method generates a name based on the name of the calling function or method.

`handler`  

A handler to be called shortly before the app’s remaining background time reaches 0. Use this handler to clean up and mark the end of the background task. Failure to end the task explicitly will result in the termination of the app. The system calls the handler synchronously on the main thread, blocking the app’s suspension momentarily.

## Return Value

A unique identifier for the new background task. You must pass this value to the endBackgroundTask(_:) method to mark the end of this task. This method returns invalid if running in the background isn’t possible.

## Mentioned in 

Extending your app’s background execution time

## Discussion

This method requests additional background execution time for your app. Call this method when leaving a task unfinished might be detrimental to your app’s user experience. For example, call this method before writing data to a file to prevent the system from suspending your app while the operation is in progress. For background tasks requiring more time, use Background Tasks.

Call this method as early as possible before starting your task, preferably before your app actually enters the background. The method requests the task assertion for your app asynchronously. If you call this method shortly before your app is due to be suspended, there’s a chance that the system might suspend your app before that task assertion is granted. For example, don’t call this method at the very end of your applicationDidEnterBackground(_:) method and expect your app to continue running. If the system is unable to grant the task assertion, it calls your expiration handler.

Each call to this method must be balanced by a matching call to the endBackgroundTask(_:) method. Apps running background tasks have a finite amount of time in which to run them. (You can find out the maximum background time available using the backgroundTimeRemaining property.) If you don’t call endBackgroundTask(_:) for each task before time expires, the system kills the app. If you provide a block object in the handler parameter, the system calls your handler before time expires to give you a chance to end the task.

You can call this method at any point in your app’s execution. You may also call this method multiple times to mark the beginning of several background tasks that run in parallel. However, each task must be ended separately. You identify a given task using the value returned by this method.

This method can be safely called on a non-main thread. To extend the execution time of an app extension, use the performExpiringActivity(withReason:using:) method of ProcessInfo instead.

## See Also

### Related Documentation

Background Tasks

Request the system to launch your app in the background to run tasks.

### Managing background tasks

var backgroundRefreshStatus: UIBackgroundRefreshStatus

Indicates whether the app can refresh content when running in the background.

enum UIBackgroundRefreshStatus

Constants that indicate whether background execution is enabled for the app.

class let backgroundRefreshStatusDidChangeNotification: NSNotification.Name

A notification that posts when the app’s status for downloading content in the background changes.

func beginBackgroundTask(expirationHandler: (() -> Void)?) -> UIBackgroundTaskIdentifier

Marks the start of a task that should continue if the app enters the background.

func endBackgroundTask(UIBackgroundTaskIdentifier)

Marks the end of a specific long-running background task.

struct UIBackgroundTaskIdentifier

A unique token that identifies a request to run in the background.

var backgroundTimeRemaining: TimeInterval

The maximum amount of time remaining for the app to run in the background.

