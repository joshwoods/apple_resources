

- CarPlay
- CPTemplateApplicationSceneDelegate
-  templateApplicationScene(\_:didConnect:to:) 

Instance Method

# templateApplicationScene(\_:didConnect:to:)

Tells the delegate about the addition of a CarPlay scene to your navigation app.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
optional func templateApplicationScene(
    _ templateApplicationScene: CPTemplateApplicationScene,
    didConnect interfaceController: CPInterfaceController,
    to window: CPWindow
)
```

## Parameters 

`templateApplicationScene`  

The scene connecting to the app.

`interfaceController`  

The interface controller for managing the user interface of this scene.

`window`  

The window where the app draws the map content.

## Mentioned in 

Displaying Content in CarPlay

## Discussion

CarPlay calls this method when it launches your navigation app and connects the scene. Create an instance of your map-drawing view controller and assign it to the window’s root view controller. Use the interface controller to present your user interface templates. You must set both the window’s root view controller and the scene’s root template before returning from this method.

Important

CarPlay calls this method exclusively for navigation apps. All other categories of apps must implement templateApplicationScene(_:didConnect:) instead.

## See Also

### Responding to the Scene Life Cycle

func templateApplicationScene(CPTemplateApplicationScene, didConnect: CPInterfaceController)

Tells the delegate about the addition of a CarPlay scene to the app.

func templateApplicationScene(CPTemplateApplicationScene, didDisconnectInterfaceController: CPInterfaceController)

Tells the delegate when CarPlay removes a scene from the app.

func templateApplicationScene(CPTemplateApplicationScene, didDisconnect: CPInterfaceController, from: CPWindow)

Tells the delegate when CarPlay removes a scene from your navigation app.

