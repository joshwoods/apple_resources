

- UIKit
- UIApplicationDelegate
-  applicationWillEnterForeground(\_:) 

Instance Method

# applicationWillEnterForeground(\_:)

Tells the delegate that the app is about to enter the foreground.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func applicationWillEnterForeground(_ application: UIApplication)
```

## Parameters 

`application`  

Your singleton app object.

## Discussion

Important

If you’re using scenes (see Scenes), UIKit will not call this method. Use sceneWillEnterForeground(_:) instead to prepare your app to enter the foreground. UIKit posts a willEnterForegroundNotification regardless of whether your app uses Scenes.

In iOS 4.0 and later, UIKit calls this method as part of the transition from the background to the active state. You can use this method to undo many of the changes you made to your app upon entering the background. The call to this method is invariably followed by a call to the applicationDidBecomeActive(_:) method, which then moves the app from the inactive to the active state.

UIKit also posts a willEnterForegroundNotification shortly before calling this method to give interested objects a chance to respond to the transition.

## See Also

### Responding to app life-cycle events

func applicationDidBecomeActive(UIApplication)

Tells the delegate that the app has become active.

func applicationWillResignActive(UIApplication)

Tells the delegate that the app is about to become inactive.

func applicationDidEnterBackground(UIApplication)

Tells the delegate that the app is now in the background.

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

