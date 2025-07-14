

- RealityKit
- Entity
-  HasHierarchy Implementations 

API Collection

# HasHierarchy Implementations

## Topics

### Instance Properties

var children: Entity.ChildCollection

The child entities that the entity manages.

var parent: Entity?

The parent entity.

### Instance Methods

func addChild(Entity, preservingWorldTransform: Bool)

Adds the given entity to the collection of child entities.

func removeChild(Entity, preservingWorldTransform: Bool)

Removes the given child from the entity.

func removeFromParent(preservingWorldTransform: Bool)

Removes the entity from its current parent or from the scene if it is a root entity.

func setParent(Entity?, preservingWorldTransform: Bool)

Attaches the entity as a child to the specified entity.

