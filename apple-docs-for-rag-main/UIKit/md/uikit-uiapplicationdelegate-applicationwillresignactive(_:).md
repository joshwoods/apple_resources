

- UIKit
- UIApplicationDelegate
-  applicationWillResignActive(\_:) 

Instance Method

# applicationWillResignActive(\_:)

Tells the delegate that the app is about to become inactive.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func applicationWillResignActive(_ application: UIApplication)
```

## Parameters 

`application`  

Your singleton app object.

## Mentioned in 

About the background execution sequence

## Discussion

Important

If you’re using scenes (see Scenes), UIKit will not call this method. Use sceneWillResignActive(_:) instead to pause any activity or save state. UIKit posts a willResignActiveNotification regardless of whether your app uses scenes.

UIKit calls this method to let your app know that it is about to move from the active to inactive state. The app moves to the inactive state because of temporary interruptions like an incoming phone call or SMS message, or when the user quits the app and it begins the transition to the background state. An app in the inactive state continues to run but doesn’t dispatch incoming events to responders.

Use this method to pause ongoing tasks, disable timers, and throttle down OpenGL ES frame rates. Games should use this method to pause the game. An app in the inactive state should do minimal work while it waits to transition to either the active or background state.

If your app has unsaved user data, you can save it to ensure that it isn’t lost. However, it is recommended that you save user data at appropriate points throughout the execution of your app, usually in response to specific actions. For example, save data when the user dismisses a data entry screen. Don’t rely on specific app state transitions to save all of your app’s critical data.

After calling this method, UIKit also posts a willResignActiveNotification to give interested objects a chance to respond to the transition.

## See Also

### Responding to app life-cycle events

func applicationDidBecomeActive(UIApplication)

Tells the delegate that the app has become active.

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

