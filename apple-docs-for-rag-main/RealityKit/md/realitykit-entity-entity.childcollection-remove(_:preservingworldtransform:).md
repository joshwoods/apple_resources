

- RealityKit
- Entity
- Entity.ChildCollection
-  remove(\_:preservingWorldTransform:) 

Instance Method

# remove(\_:preservingWorldTransform:)

Removes the specified child from this entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func remove(
    _ child: Entity,
    preservingWorldTransform: Bool = false
)
```

## Parameters 

`child`  

The child entity to remove from the collection.

`preservingWorldTransform`  

`true` to preserve the world transform. `false` to preserve the relative transform. (Use `true` if the entities should keep its effective location and size in the scene!)

## Discussion

Note

This may modify the order of the `ChildCollection`.

## See Also

### Removing entities

func remove(at: Int, preservingWorldTransform: Bool)

Removes the specified child from this entity.

func removeAll(preservingWorldTransforms: Bool)

func removeAll(keepCapacity: Bool, preservingWorldTransforms: Bool)

Removes all children from this entity.

