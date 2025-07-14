

- UIKit
- UISceneDelegate
-  sceneDidDisconnect(\_:) 

Instance Method

# sceneDidDisconnect(\_:)

Tells the delegate that UIKit removed a scene from your app.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
optional func sceneDidDisconnect(_ scene: UIScene)
```

## Parameters 

`scene`  

The scene that UIKit disconnected from your app.

## Mentioned in 

Presenting content on a connected display

## Discussion

Use this method to perform any final cleanup before your scene is purged from memory. For example, use it to release references to files or shared resources and to save user data.

The removal of a scene is a precursor to the destruction of that scene. UIKit disconnects a scene when the user explicitly closes it in the app switcher. UIKit may also disconnect a scene in order to reclaim memory for other processes. UIKit does not automatically disconnect a scene when the user switches to another app.

UIKit also posts a didDisconnectNotification notification in addition to calling this method.

## See Also

### Connecting and disconnecting the scene

func scene(UIScene, willConnectTo: UISceneSession, options: UIScene.ConnectionOptions)

Tells the delegate about the addition of a scene to the app.

class ConnectionOptions

A data object containing information about the reasons why UIKit created the scene.

