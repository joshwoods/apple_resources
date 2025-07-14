

- CarPlay
- CPTemplateApplicationSceneDelegate
-  templateApplicationScene(\_:didDisconnect:from:) 

Instance Method

# templateApplicationScene(\_:didDisconnect:from:)

Tells the delegate when CarPlay removes a scene from your navigation app.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
optional func templateApplicationScene(
    _ templateApplicationScene: CPTemplateApplicationScene,
    didDisconnect interfaceController: CPInterfaceController,
    from window: CPWindow
)
```

## Parameters 

`templateApplicationScene`  

The scene disconnecting from the app.

`interfaceController`  

The interface controller for managing the user interface of this scene.

`window`  

The window where the app draws the map content.

## Discussion

CarPlay calls this method after it disconnects the scene. You can use it to perform any cleanup.

Important

CarPlay calls this method exclusively for navigation apps. All other categories of apps must implement templateApplicationScene(_:didDisconnectInterfaceController:) instead.

## See Also

### Responding to the Scene Life Cycle

func templateApplicationScene(CPTemplateApplicationScene, didConnect: CPInterfaceController)

Tells the delegate about the addition of a CarPlay scene to the app.

func templateApplicationScene(CPTemplateApplicationScene, didConnect: CPInterfaceController, to: CPWindow)

Tells the delegate about the addition of a CarPlay scene to your navigation app.

func templateApplicationScene(CPTemplateApplicationScene, didDisconnectInterfaceController: CPInterfaceController)

Tells the delegate when CarPlay removes a scene from the app.

