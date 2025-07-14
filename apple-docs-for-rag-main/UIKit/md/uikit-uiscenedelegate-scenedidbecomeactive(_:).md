

- UIKit
- UISceneDelegate
-  sceneDidBecomeActive(\_:) 

Instance Method

# sceneDidBecomeActive(\_:)

Tells the delegate that the scene became active and is now responding to user events.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
optional func sceneDidBecomeActive(_ scene: UIScene)
```

## Parameters 

`scene`  

The scene that became active and is now responding to user events.

## Discussion

To use this method, you must implement the UISceneDelegate protocol and configure scenes for your app (see Specifying the scenes your app supports).

Use this method to prepare your scene to be onscreen. UIKit calls this method after loading the interface for your scene, but before that interface appears onscreen. Use it to refresh the contents of views, start timers, or increase frame rates for your UI.

In addition to calling this method, UIKit posts a didActivateNotification and a didBecomeActiveNotification.

For more information on what to do when your app becomes active, see Preparing your UI to run in the foreground.

Note

When you implement this method and enable scenes, UIKit calls this method but does not call the applicationDidBecomeActive(_:) method on UIApplicationDelegate.

## See Also

### Transitioning to the foreground

func sceneWillEnterForeground(UIScene)

Tells the delegate that the scene is about to begin running in the foreground and become visible to the user.

