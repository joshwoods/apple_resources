

- RealityKit
- Entity
-  parent 

Instance Property

# parent

The parent entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
var parent: Entity? { get }
```

## Discussion

An entity has at most one parent entity. If an entity isn’t part of a hierarchy, or if it is a root entity, the parent property is `nil`.

Use the setParent(_:preservingWorldTransform:) method to change an entity’s parent. Use the removeFromParent(preservingWorldTransform:) method to remove the parent. These methods automatically update the corresponding children collections of the new and old parent.

## See Also

### Relating entities

func setParent(Entity?, preservingWorldTransform: Bool)

Attaches the entity as a child to the specified entity.

func removeFromParent(preservingWorldTransform: Bool)

Removes the entity from its current parent or from the scene if it is a root entity.

var children: Entity.ChildCollection

The child entities that the entity manages.

func addChild(Entity, preservingWorldTransform: Bool)

Adds the given entity to the collection of child entities.

func removeChild(Entity, preservingWorldTransform: Bool)

Removes the given child from the entity.

struct ChildCollection

A collection of child entities.

protocol HasHierarchy

An interface that provides access to a parent entity and child entities.

