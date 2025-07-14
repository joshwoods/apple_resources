

- RealityKit
- Entity
-  addChild(\_:preservingWorldTransform:) 

Instance Method

# addChild(\_:preservingWorldTransform:)

Adds the given entity to the collection of child entities.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func addChild(
    _ entity: Entity,
    preservingWorldTransform: Bool = false
)
```

## Parameters 

`entity`  

`preservingWorldTransform`  

A Boolean that you set to `true` to preserve the entity’s world transform, or `false` to preserve its relative transform. Use `true` when you want a model to keep its effective location and size within a scene.

## Discussion

See the HasHierarchy protocol’s definition of addChild(_:preservingWorldTransform:) for more information.

## See Also

### Relating entities

var parent: Entity?

The parent entity.

func setParent(Entity?, preservingWorldTransform: Bool)

Attaches the entity as a child to the specified entity.

func removeFromParent(preservingWorldTransform: Bool)

Removes the entity from its current parent or from the scene if it is a root entity.

var children: Entity.ChildCollection

The child entities that the entity manages.

func removeChild(Entity, preservingWorldTransform: Bool)

Removes the given child from the entity.

struct ChildCollection

A collection of child entities.

protocol HasHierarchy

An interface that provides access to a parent entity and child entities.

