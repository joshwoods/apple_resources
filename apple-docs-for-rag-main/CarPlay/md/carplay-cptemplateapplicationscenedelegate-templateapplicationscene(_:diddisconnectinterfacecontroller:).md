

- CarPlay
- CPTemplateApplicationSceneDelegate
-  templateApplicationScene(\_:didDisconnectInterfaceController:) 

Instance Method

# templateApplicationScene(\_:didDisconnectInterfaceController:)

Tells the delegate when CarPlay removes a scene from the app.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
optional func templateApplicationScene(
    _ templateApplicationScene: CPTemplateApplicationScene,
    didDisconnectInterfaceController interfaceController: CPInterfaceController
)
```

## Parameters 

`templateApplicationScene`  

The scene disconnecting from the app.

`interfaceController`  

The interface controller for managing the user interface of this scene.

## Discussion

CarPlay calls this method after it disconnects the scene. You can use it to perform any cleanup.

Important

CarPlay doesn’t call this method for navigation apps. You must implement templateApplicationScene(_:didDisconnect:from:) instead.

## See Also

### Responding to the Scene Life Cycle

func templateApplicationScene(CPTemplateApplicationScene, didConnect: CPInterfaceController)

Tells the delegate about the addition of a CarPlay scene to the app.

func templateApplicationScene(CPTemplateApplicationScene, didConnect: CPInterfaceController, to: CPWindow)

Tells the delegate about the addition of a CarPlay scene to your navigation app.

func templateApplicationScene(CPTemplateApplicationScene, didDisconnect: CPInterfaceController, from: CPWindow)

Tells the delegate when CarPlay removes a scene from your navigation app.

