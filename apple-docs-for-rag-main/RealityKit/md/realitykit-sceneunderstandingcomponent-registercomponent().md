

- RealityKit
- SceneUnderstandingComponent
-  registerComponent() 

Type Method

# registerComponent()

Registers a new component type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
static func registerComponent()
```

## Discussion

Call the `registerComponent()` method once for every custom component type that you use in your app before you use it. You don’t need to call the method for built-in component types, like ModelComponent or AnchoringComponent.

## See Also

### Managing the component

var entityType: SceneUnderstandingComponent.EntityType?

The type of real-world objects that the component models.

enum EntityType

Types of real-world objects that a scene-understanding component models.

