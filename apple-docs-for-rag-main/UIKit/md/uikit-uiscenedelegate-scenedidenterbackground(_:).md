

- UIKit
- UISceneDelegate
-  sceneDidEnterBackground(\_:) 

Instance Method

# sceneDidEnterBackground(\_:)

Tells the delegate that the scene is running in the background and is no longer onscreen.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
optional func sceneDidEnterBackground(_ scene: UIScene)
```

## Parameters 

`scene`  

The scene that entered the background.

## Discussion

To use this method, you must implement the UISceneDelegate protocol and configure scenes for your app (see Specifying the scenes your app supports).

Use this method to reduce your scene’s memory usage, free up any shared resources, and clean up your scene’s user interface. Shortly after this method returns, UIKit takes a snapshot of your scene’s interface for display in the app switcher. Make sure your interface doesn’t contain sensitive user information.

In addition to calling this method, UIKit posts a didEnterBackgroundNotification notification from UIApplication and UIScene.

For more information about what to do when your app enters the background, see Preparing your UI to run in the background.

Note

When you implement this method and enable scenes, UIKit calls this method but does not call the applicationDidEnterBackground(_:) method on UIApplicationDelegate.

## See Also

### Transitioning to the background

func sceneWillResignActive(UIScene)

Tells the delegate that the scene is about to resign the active state and stop responding to user events.

