

- RealityKit
- Entity
- Entity.ChildCollection
-  append(contentsOf:preservingWorldTransforms:) 

Instance Method

# append(contentsOf:preservingWorldTransforms:)

Moves all `children` to be children of this entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func append(
    contentsOf children: Entity.ChildCollection,
    preservingWorldTransforms: Bool = false
)
```

## Parameters 

`children`  

The child entities to add to the collection.

`preservingWorldTransforms`  

`true` to preserve the world transform. `false` to preserve the relative transform. (Use `true` if the entities should keep its effective location and size in the scene!)

