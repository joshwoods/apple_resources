

- RealityKit
- Entity
- Entity.ChildCollection
-  removeAll(keepCapacity:preservingWorldTransforms:) 

Instance Method

# removeAll(keepCapacity:preservingWorldTransforms:)

Removes all children from this entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func removeAll(
    keepCapacity: Bool = false,
    preservingWorldTransforms: Bool = false
)
```

## Parameters 

`keepCapacity`  

`true` to keep the memory reserved for storing the children. `false` to free the reserved memory.

`preservingWorldTransforms`  

`true` to preserve the world transform. `false` to preserve the relative transform. (Use `true` if the entities should keep its effective location and size in the scene!)

## See Also

### Removing entities

func remove(Entity, preservingWorldTransform: Bool)

Removes the specified child from this entity.

func remove(at: Int, preservingWorldTransform: Bool)

Removes the specified child from this entity.

func removeAll(preservingWorldTransforms: Bool)

