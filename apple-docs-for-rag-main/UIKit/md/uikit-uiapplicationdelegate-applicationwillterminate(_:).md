

- UIKit
- UIApplicationDelegate
-  applicationWillTerminate(\_:) 

Instance Method

# applicationWillTerminate(\_:)

Tells the delegate when the app is about to terminate.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func applicationWillTerminate(_ application: UIApplication)
```

## Parameters 

`application`  

Your singleton app object.

## Discussion

This method lets your app know that it is about to be terminated and purged from memory entirely. You should use this method to perform any final clean-up tasks for your app, such as freeing shared resources, saving user data, and invalidating timers. Your implementation of this method has approximately five seconds to perform any tasks and return. If the method does not return before time expires, the system may terminate the process altogether.

For apps that do not support background execution or are linked against iOS 3.x or earlier, this method is always called when the user quits the app. For apps that support background execution, this method is generally not called when the user quits the app because the app simply moves to the background in that case. However, this method may be called in situations where the app is running in the background (not suspended) and the system needs to terminate it for some reason.

After calling this method, the app also posts a willTerminateNotification notification to give interested objects a chance to respond to the transition.

## See Also

### Related Documentation

func application(UIApplication, didFinishLaunchingWithOptions: [UIApplication.LaunchOptionsKey : Any]?) -> Bool

Tells the delegate that the launch process is almost done and the app is almost ready to run.

### Responding to app life-cycle events

func applicationDidBecomeActive(UIApplication)

Tells the delegate that the app has become active.

func applicationWillResignActive(UIApplication)

Tells the delegate that the app is about to become inactive.

func applicationDidEnterBackground(UIApplication)

Tells the delegate that the app is now in the background.

func applicationWillEnterForeground(UIApplication)

Tells the delegate that the app is about to enter the foreground.

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

