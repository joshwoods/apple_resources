

- UIKit
- UISceneDelegate
-  sceneWillResignActive(\_:) 

Instance Method

# sceneWillResignActive(\_:)

Tells the delegate that the scene is about to resign the active state and stop responding to user events.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
optional func sceneWillResignActive(_ scene: UIScene)
```

## Parameters 

`scene`  

The scene that is about to stop responding to user events.

## Discussion

To use this method, you must implement the UISceneDelegate protocol and configure scenes for your app (see Specifying the scenes your app supports).

UIKit calls this method for temporary interruptions, such as when displaying system alerts. It also calls the method before transitioning your app to the background state.

Use this method to quiet your interface and prepare it to stop interacting with the user. Specifically, pause ongoing tasks, disable timers, and decrease frame rates or stop updating your interface altogether. Games should use this method to pause the game. By the time this method returns, your app should be doing minimal work while it waits to transition to the background or to the foreground again.

If your scene has unsaved user data, save that data in this method to ensure that it isn’t lost. However, never save data solely from this method. Instead, save it at appropriate points from your view controllers, usually in response to user actions. For example, save data when the user dismisses a data-entry screen. Don’t rely on specific app transitions to save all of your app’s critical data.

In addition to calling this method, UIKit posts a willDeactivateNotification and a willResignActiveNotification.

For more information about what to do when your app resigns the active state, see Preparing your UI to run in the background.

Note

When you implement this method and enable scenes, UIKit calls this method but does not call the applicationWillResignActive(_:) method on UIApplicationDelegate.

## See Also

### Transitioning to the background

func sceneDidEnterBackground(UIScene)

Tells the delegate that the scene is running in the background and is no longer onscreen.

