

- RealityKit
- HasHierarchy
-  removeFromParent(preservingWorldTransform:) 

Instance Method

# removeFromParent(preservingWorldTransform:)

Removes the entity from its current parent or from the scene if it is a root entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func removeFromParent(preservingWorldTransform: Bool = false)
```

## Parameters 

`preservingWorldTransform`  

A Boolean that you set to `true` to preserve the entity’s world transform, or `false` to preserve its relative transform. Use `true` when you want a model to keep its effective location and size within a scene.

## Discussion

This method behaves like the setParent(_:preservingWorldTransform:) method with a value of `nil` for the `parent` parameter, except that method has no effect on root entities. A root entity is one that is stored in a scene’s anchors collection.

The children collections of any modified parent entities are automatically updated as well.

## See Also

### Managing the parent

var parent: Entity?

The parent entity.

func setParent(Entity?, preservingWorldTransform: Bool)

Attaches the entity as a child to the specified entity.

