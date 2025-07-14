

- CarPlay
- CPTemplateApplicationSceneDelegate
-  templateApplicationScene(\_:didConnect:) 

Instance Method

# templateApplicationScene(\_:didConnect:)

Tells the delegate about the addition of a CarPlay scene to the app.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
optional func templateApplicationScene(
    _ templateApplicationScene: CPTemplateApplicationScene,
    didConnect interfaceController: CPInterfaceController
)
```

## Parameters 

`templateApplicationScene`  

The scene connecting to the app.

`interfaceController`  

The interface controller for managing the user interface of this scene.

## Mentioned in 

Displaying Content in CarPlay

## Discussion

CarPlay calls this method when it launches your app and connects the scene. Use the interface controller to present your user interface templates. You must set the scene’s root template before returning from this method.

Important

Navigation apps must implement templateApplicationScene(_:didConnect:to:) instead so they can access the window where they draw their map content.

## See Also

### Responding to the Scene Life Cycle

func templateApplicationScene(CPTemplateApplicationScene, didConnect: CPInterfaceController, to: CPWindow)

Tells the delegate about the addition of a CarPlay scene to your navigation app.

func templateApplicationScene(CPTemplateApplicationScene, didDisconnectInterfaceController: CPInterfaceController)

Tells the delegate when CarPlay removes a scene from the app.

func templateApplicationScene(CPTemplateApplicationScene, didDisconnect: CPInterfaceController, from: CPWindow)

Tells the delegate when CarPlay removes a scene from your navigation app.

