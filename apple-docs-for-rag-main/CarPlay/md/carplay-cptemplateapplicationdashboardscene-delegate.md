

- CarPlay
- CPTemplateApplicationDashboardScene
-  delegate 

Instance Property

# delegate

The object that receives the dashboard scene’s life-cycle events.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+

``` source
@MainActor
var delegate: (any CPTemplateApplicationDashboardSceneDelegate)? { get set }
```

## Discussion

Use this property to access the delegate object CarPlay creates from the class name you provide in the scene manifest of your app’s `Info.plist` file. You can update this property at runtime to provide an alternate delegate object.

## See Also

### Responding to the Dashboard Scene Life Cycle

protocol CPTemplateApplicationDashboardSceneDelegate

The methods for responding to the life-cycle events of your navigation app’s dashboard scene.

