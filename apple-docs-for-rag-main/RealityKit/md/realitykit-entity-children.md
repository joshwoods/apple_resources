

- RealityKit
- Entity
-  children 

Instance Property

# children

The child entities that the entity manages.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var children: Entity.ChildCollection { get set }
```

## Discussion

An entity can have any number of child entities.

Use the addChild(_:preservingWorldTransform:) method to add a child to an entity. Use the removeChild(_:preservingWorldTransform:) method to remove one from an entity. These methods automatically update the parent properties of the child entities.

## See Also

### Relating entities

var parent: Entity?

The parent entity.

func setParent(Entity?, preservingWorldTransform: Bool)

Attaches the entity as a child to the specified entity.

func removeFromParent(preservingWorldTransform: Bool)

Removes the entity from its current parent or from the scene if it is a root entity.

func addChild(Entity, preservingWorldTransform: Bool)

Adds the given entity to the collection of child entities.

func removeChild(Entity, preservingWorldTransform: Bool)

Removes the given child from the entity.

struct ChildCollection

A collection of child entities.

protocol HasHierarchy

An interface that provides access to a parent entity and child entities.

