

- UIKit
- UIApplication
-  willTerminateNotification 

Type Property

# willTerminateNotification

A notification that posts when the app is about to terminate.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
nonisolated
class let willTerminateNotification: NSNotification.Name
```

## Discussion

This notification is associated with the delegate applicationWillTerminate(_:) method. This notification does not contain a `userInfo` dictionary.

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

class let willResignActiveNotification: NSNotification.Name

A notification that posts when the app is no longer active and loses focus.

