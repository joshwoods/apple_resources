

- UIKit
- UISceneDelegate
-  scene(\_:willConnectTo:options:) 

Instance Method

# scene(\_:willConnectTo:options:)

Tells the delegate about the addition of a scene to the app.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
optional func scene(
    _ scene: UIScene,
    willConnectTo session: UISceneSession,
    options connectionOptions: UIScene.ConnectionOptions
)
```

## Parameters 

`scene`  

The scene object being connected to your app.

`session`  

The session object containing details about the scene’s configuration.

`connectionOptions`  

Additional options for configuring the scene. Use the information in this object to handle actions that caused the creation of the scene, for example, to respond to a quick action selected by the user.

## Mentioned in 

About the app launch sequence

Presenting content on a connected display

## Discussion

This method is called when your app creates or restores an instance of your user interface.

When the user or your app requests a new instance of your user interface, UIKit creates an appropriate scene object and connects it to your app. Use this method to respond to the addition of the new scene and to begin loading any data that the scene needs to display.

When your app responds to scene activations requests, for example, by using requestSceneSessionActivation(_:userActivity:options:errorHandler:), the user activity is in the userActivities set provided by options.

When the user reactivates an instance of your user interface, UIKit creates a scene object and populates it with saved state, provided by stateRestorationActivity(for:). When your app restores state, the user activity is presented in the stateRestorationActivity property of session.

In addition to calling this method, UIKit also posts a willConnectNotification notification.

## Topics

### Window Scenes

Supporting multiple windows on iPad

Support side-by-side instances of your app’s interface and create new windows.

## See Also

### Connecting and disconnecting the scene

func sceneDidDisconnect(UIScene)

Tells the delegate that UIKit removed a scene from your app.

class ConnectionOptions

A data object containing information about the reasons why UIKit created the scene.

