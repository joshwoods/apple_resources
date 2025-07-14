

- UIKit
- UIApplicationDelegate
-  applicationDidBecomeActive(\_:) 

Instance Method

# applicationDidBecomeActive(\_:)

Tells the delegate that the app has become active.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func applicationDidBecomeActive(_ application: UIApplication)
```

## Parameters 

`application`  

Your singleton app object.

## Discussion

Important

If you’re using scenes (see Scenes), UIKit will not call this method. Use sceneDidBecomeActive(_:) instead to restart any tasks or refresh your app’s user interface. UIKit posts a didBecomeActiveNotification regardless of whether your app uses scenes.

UIKit calls this method to let your app know that it moved from the inactive to active state. The app moves to the active state because it was launched by the user or the system, or because the user ignores an interruption (like an incoming phone call or SMS message) that sent the app temporarily to the inactive state.

Use this method to restart any tasks that were paused (or not yet started) while the app was inactive. For example, use it to restart timers or throttle up OpenGL ES frame rates. If your app was previously in the background, you can also use it to refresh your app’s user interface.

After calling this method, UIKit posts a didBecomeActiveNotification to give interested objects a chance to respond to the transition.

## See Also

### Responding to app life-cycle events

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

class let willTerminateNotification: NSNotification.Name

A notification that posts when the app is about to terminate.

