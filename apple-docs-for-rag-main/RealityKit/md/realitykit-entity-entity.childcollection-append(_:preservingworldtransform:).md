

- RealityKit
- Entity
- Entity.ChildCollection
-  append(\_:preservingWorldTransform:) 

Instance Method

# append(\_:preservingWorldTransform:)

Adds the specified entity as a child to this entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func append(
    _ child: Entity,
    preservingWorldTransform: Bool = false
)
```

## Parameters 

`child`  

The child entity to add to the collection.

`preservingWorldTransform`  

`true` to preserve the world transform. `false` to preserve the relative transform. (Use `true` if the model should keep its effective location and size in the scene!)

## See Also

### Adding entities

func append&lt;S>(contentsOf: S, preservingWorldTransforms: Bool)

Adds the specified list of entity as children to this entity.

func append(contentsOf: [Entity], preservingWorldTransforms: Bool)

Adds the specified list of entity as children to this entity.

