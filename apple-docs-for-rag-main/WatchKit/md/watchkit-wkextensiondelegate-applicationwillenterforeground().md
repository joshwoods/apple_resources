

- WatchKit
- WKExtensionDelegate
-  applicationWillEnterForeground() 

Instance Method

# applicationWillEnterForeground()

Tells the delegate that the app is about to transition from the background to the foreground.

watchOS 2.0+

``` source
@MainActor
optional func applicationWillEnterForeground()
```

## Mentioned in 

Working with the watchOS app life cycle

Handling Common State Transitions

## Discussion

The system calls this method when the app transitions from the background to the foreground. Override this method to undo many of the changes you made to your app upon entering the background. The call to this method is invariably followed by a call to the applicationDidBecomeActive() method, as the app moves from the inactive to the active state.

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

func applicationWillResignActive()

Tells the delegate that the system is about to deactivate the watchOS app.

func applicationDidEnterBackground()

Tells the delegate that the app has transitioned from the foreground to the background.

func deviceOrientationDidChange()

Tells the delegate that the device’s orientation has changed.

