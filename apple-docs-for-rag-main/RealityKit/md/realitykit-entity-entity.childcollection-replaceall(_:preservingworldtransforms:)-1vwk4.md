

- RealityKit
- Entity
- Entity.ChildCollection
-  replaceAll(\_:preservingWorldTransforms:) 

Instance Method

# replaceAll(\_:preservingWorldTransforms:)

Removes all children from this entity and adds the specified list of entities as the new children.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func replaceAll(
    _ children: S,
    preservingWorldTransforms: Bool = false
) where S : Sequence, S.Element : Entity
```

## Parameters 

`children`  

The list of the new children.

`preservingWorldTransforms`  

`true` to preserve the world transform. `false` to preserve the relative transform. (Use `true` if the entities should keep its effective location and size in the scene!)

## See Also

### Replacing entities

func replaceAll([Entity], preservingWorldTransforms: Bool)

Removes all children from this entity and adds the specified list of entities as the new children.

