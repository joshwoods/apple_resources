

- RealityKit
- HasHierarchy
-  setParent(\_:preservingWorldTransform:) 

Instance Method

# setParent(\_:preservingWorldTransform:)

Attaches the entity as a child to the specified entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func setParent(
    _ parent: Entity?,
    preservingWorldTransform: Bool = false
)
```

## Parameters 

`parent`  

The new parent entity. Use `nil` to detach the entity from its current parent.

`preservingWorldTransform`  

A Boolean that you set to `true` to preserve the entity’s world transform, or `false` to preserve its relative transform. Use `true` when you want a model to keep its effective location and size within a scene.

## Discussion

Attaching an entity to a new parent automatically detaches it from its old parent.

The children collections of both the old and new parent are automatically updated as well.

Important

On visionOS, only use `preservingWorldTransform` when moving an entity within the same `AnchorEntity`, `ImmersiveSpace` or SwiftUI `WindowGroup` hierarchy. Moving entities across these hierarchy boundaries while `preservingWorldTransform` is set to `true`, is not supported.

## See Also

### Managing the parent

var parent: Entity?

The parent entity.

func removeFromParent(preservingWorldTransform: Bool)

Removes the entity from its current parent or from the scene if it is a root entity.

