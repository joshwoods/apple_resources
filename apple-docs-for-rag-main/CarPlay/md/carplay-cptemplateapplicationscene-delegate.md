

- CarPlay
- CPTemplateApplicationScene
-  delegate 

Instance Property

# delegate

The object that receives the scene’s life-cycle events.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
@MainActor
var delegate: (any CPTemplateApplicationSceneDelegate)? { get set }
```

## Discussion

Use this property to access the delegate object CarPlay creates from the class name you provide in the scene manifest of your app’s `Info.plist` file.

## See Also

### Responding to the Scene Life Cycle

protocol CPTemplateApplicationSceneDelegate

The methods for responding to the life cycle events of your app’s scene.

