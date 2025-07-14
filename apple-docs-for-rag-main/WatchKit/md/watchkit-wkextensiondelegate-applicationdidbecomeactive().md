

- WatchKit
- WKExtensionDelegate
-  applicationDidBecomeActive() 

Instance Method

# applicationDidBecomeActive()

Tells the delegate that the watchOS app is visible and processing events.

watchOS 2.0+

``` source
@MainActor
optional func applicationDidBecomeActive()
```

## Mentioned in 

Working with the watchOS app life cycle

Handling Common State Transitions

## Discussion

WatchKit calls this method to let you know that your app transitioned from the inactive to the active state. Use this method to start any tasks that were paused or not yet started while the app was inactive. For example, you could use it to start timers. You can also use it to gather information needed to configure your app’s initial user interface.

Note

When creating an app that uses the SwiftUI App protocol to manage your life cycle, use the onChange(of:perform:) modifier and the scenePhase environment value to monitor life cycle changes when possible. For more information, see Building a watchOS app.

## See Also

### Monitoring state changes

Working with the watchOS app life cycle

Learn how the watchOS app life cycle operates and responds to life cycle notification methods.

func applicationDidFinishLaunching()

Tells the delegate that the launch process is almost done and the extension is almost ready to run.

func applicationWillResignActive()

Tells the delegate that the system is about to deactivate the watchOS app.

func applicationWillEnterForeground()

Tells the delegate that the app is about to transition from the background to the foreground.

func applicationDidEnterBackground()

Tells the delegate that the app has transitioned from the foreground to the background.

func deviceOrientationDidChange()

Tells the delegate that the device’s orientation has changed.

