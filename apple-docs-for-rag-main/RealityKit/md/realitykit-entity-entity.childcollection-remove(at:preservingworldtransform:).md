

- RealityKit
- Entity
- Entity.ChildCollection
-  remove(at:preservingWorldTransform:) 

Instance Method

# remove(at:preservingWorldTransform:)

Removes the specified child from this entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func remove(
    at index: Int,
    preservingWorldTransform: Bool = false
)
```

## Parameters 

`index`  

The index of the child entity to remove from the collection.

`preservingWorldTransform`  

`true` to preserve the world transform. `false` to preserve the relative transform. (Use `true` if the entities should keep its effective location and size in the scene!)

## Discussion

Note

This may modify the order of the `ChildCollection`.

## See Also

### Removing entities

func remove(Entity, preservingWorldTransform: Bool)

Removes the specified child from this entity.

func removeAll(preservingWorldTransforms: Bool)

func removeAll(keepCapacity: Bool, preservingWorldTransforms: Bool)

Removes all children from this entity.

