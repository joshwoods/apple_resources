

- UIKit
- UIApplication
-  willResignActiveNotification 

Type Property

# willResignActiveNotification

A notification that posts when the app is no longer active and loses focus.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
nonisolated
class let willResignActiveNotification: NSNotification.Name
```

## Discussion

An app is active when it is receiving events. An active app can be said to have focus. It gains focus after being launched, loses focus when an overlay window pops up or when the device is locked, and gains focus when the device is unlocked.

## See Also

### Responding to app life-cycle events

func applicationDidBecomeActive(UIApplication)

Tells the delegate that the app has become active.

func applicationWillResignActive(UIApplication)

Tells the delegate that the app is about to become inactive.

func applicationDidEnterBackground(UIApplication)

Tells the delegate that the app is now in the background.

func applicationWillEnterForeground(UIApplication)

Tells the delegate that the app is about to enter the foreground.

func applicationWillTerminate(UIApplication)

Tells the delegate when the app is about to terminate.

class let didBecomeActiveNotification: NSNotification.Name

A notification that posts when the app becomes active.

class let didEnterBackgroundNotification: NSNotification.Name

A notification that posts when the app enters the background.

class let willEnterForegroundNotification: NSNotification.Name

A notification that posts shortly before an app leaves the background state on its way to becoming the active app.

class let willTerminateNotification: NSNotification.Name

A notification that posts when the app is about to terminate.

