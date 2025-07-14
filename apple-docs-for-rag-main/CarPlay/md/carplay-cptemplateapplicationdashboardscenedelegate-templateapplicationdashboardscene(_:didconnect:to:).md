

- CarPlay
- CPTemplateApplicationDashboardSceneDelegate
-  templateApplicationDashboardScene(\_:didConnect:to:) 

Instance Method

# templateApplicationDashboardScene(\_:didConnect:to:)

Tells the delegate about the addition of a CarPlay Dashboard scene to your navigation app.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
optional func templateApplicationDashboardScene(
    _ templateApplicationDashboardScene: CPTemplateApplicationDashboardScene,
    didConnect dashboardController: CPDashboardController,
    to window: UIWindow
)
```

## Parameters 

`templateApplicationDashboardScene`  

The scene connecting to the app.

`dashboardController`  

The controller that manages the scene’s dashboard shortcut buttons.

`window`  

The window where your app draws its map content.

## Mentioned in 

Displaying Content in CarPlay

## Discussion

CarPlay calls this method when it connects a dashboard scene to your navigation app. Create an instance of your map-drawing view controller and assign it as the window’s root view controller. Use the dashboard controller to provide up to two shortcut buttons to display instead of your map content when there’s no active navigation session.

## See Also

### Responding to the Scene Life Cycle

func templateApplicationDashboardScene(CPTemplateApplicationDashboardScene, didDisconnect: CPDashboardController, from: UIWindow)

Tells the delegate when CarPlay removes the dashboard scene from your navigation app.

