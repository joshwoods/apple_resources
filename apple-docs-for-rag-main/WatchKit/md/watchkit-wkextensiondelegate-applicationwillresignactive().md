

- WatchKit
- WKExtensionDelegate
-  applicationWillResignActive() 

Instance Method

# applicationWillResignActive()

Tells the delegate that the system is about to deactivate the watchOS app.

watchOS 2.0+

``` source
@MainActor
optional func applicationWillResignActive()
```

## Mentioned in 

Working with the watchOS app life cycle

Handling Common State Transitions

## Discussion

WatchKit calls this method after your app launches and before it exits. Use this method to pause any active tasks. For example, you could use it to stop any active timers. An app in the inactive state should do minimal work while it waits to transition to the active or not running state.

If your app has unsaved user data, you can save it here to ensure that it isn’t lost. However, it’s a good idea to save user data at appropriate points throughout the execution of your app, usually in response to user actions. Don’t rely on specific app state transitions to save all of your app’s critical data.

Note

When creating an app that uses the SwiftUI App protocol to manage your life cycle, use the onChange(of:perform:) modifier and the scenePhase environment value to monitor life cycle changes when possible. For more information, see Building a watchOS app.

## See Also

### Monitoring state changes

Working with the watchOS app life cycle

Learn how the watchOS app life cycle operates and responds to life cycle notification methods.

func applicationDidFinishLaunching()

Tells the delegate that the launch process is almost done and the extension is almost ready to run.

func applicationDidBecomeActive()

Tells the delegate that the watchOS app is visible and processing events.

func applicationWillEnterForeground()

Tells the delegate that the app is about to transition from the background to the foreground.

func applicationDidEnterBackground()

Tells the delegate that the app has transitioned from the foreground to the background.

func deviceOrientationDidChange()

Tells the delegate that the device’s orientation has changed.

