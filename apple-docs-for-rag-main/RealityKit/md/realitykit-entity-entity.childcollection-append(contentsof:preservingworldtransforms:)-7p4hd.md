

- RealityKit
- Entity
- Entity.ChildCollection
-  append(contentsOf:preservingWorldTransforms:) 

Instance Method

# append(contentsOf:preservingWorldTransforms:)

Adds the specified list of entity as children to this entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func append(
    contentsOf array: [Entity],
    preservingWorldTransforms: Bool = false
)
```

## Parameters 

`array`  

The child entities to add to the collection.

`preservingWorldTransforms`  

`true` to preserve the world transform. `false` to preserve the relative transform. (Use `true` if the entities should keep its effective location and size in the scene!)

## See Also

### Adding entities

func append&lt;S>(contentsOf: S, preservingWorldTransforms: Bool)

Adds the specified list of entity as children to this entity.

func append(Entity, preservingWorldTransform: Bool)

Adds the specified entity as a child to this entity.

