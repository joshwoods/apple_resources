

- WatchKit
- WKExtensionDelegate
-  applicationDidEnterBackground() 

Instance Method

# applicationDidEnterBackground()

Tells the delegate that the app has transitioned from the foreground to the background.

watchOS 2.0+

``` source
@MainActor
optional func applicationDidEnterBackground()
```

## Mentioned in 

Working with the watchOS app life cycle

Handling Common State Transitions

## Discussion

Override this method to release shared resources, invalidate timers, and store enough app state information to restore your app to its current state if it’s purged from memory. You have only a few seconds to complete these actions and return.

The system typically suspends your app shortly after this method returns; therefore, don’t call any asynchronous methods from your applicationDidEnterBackground() implementation. Asynchronous methods may not be able to complete before the app is suspended.

Additionally, the system may purge suspended apps at any time to make room for other apps. You aren’t notified when an app is purged from memory. The applicationDidEnterBackground() method is your last chance to perform any cleanup before the app terminates.

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

func applicationWillEnterForeground()

Tells the delegate that the app is about to transition from the background to the foreground.

func deviceOrientationDidChange()

Tells the delegate that the device’s orientation has changed.

