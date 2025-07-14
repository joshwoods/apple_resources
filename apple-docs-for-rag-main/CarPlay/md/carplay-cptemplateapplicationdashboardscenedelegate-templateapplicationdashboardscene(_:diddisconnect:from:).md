

- CarPlay
- CPTemplateApplicationDashboardSceneDelegate
-  templateApplicationDashboardScene(\_:didDisconnect:from:) 

Instance Method

# templateApplicationDashboardScene(\_:didDisconnect:from:)

Tells the delegate when CarPlay removes the dashboard scene from your navigation app.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
optional func templateApplicationDashboardScene(
    _ templateApplicationDashboardScene: CPTemplateApplicationDashboardScene,
    didDisconnect dashboardController: CPDashboardController,
    from window: UIWindow
)
```

## Parameters 

`templateApplicationDashboardScene`  

The scene disconnecting from the app.

`dashboardController`  

The controller that was managing this scene’s dashboard shortcut buttons.

`window`  

The window where your app was drawing its map content.

## Discussion

CarPlay calls this method after it disconnects your dashboard scene. You can use it to perform any cleanup.

## See Also

### Responding to the Scene Life Cycle

func templateApplicationDashboardScene(CPTemplateApplicationDashboardScene, didConnect: CPDashboardController, to: UIWindow)

Tells the delegate about the addition of a CarPlay Dashboard scene to your navigation app.

