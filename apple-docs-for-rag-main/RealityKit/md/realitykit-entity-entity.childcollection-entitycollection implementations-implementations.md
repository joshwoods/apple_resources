

- RealityKit
- Entity
- Entity.ChildCollection
-  EntityCollection Implementations 

API Collection

# EntityCollection Implementations

## Topics

### Instance Methods

func append(Entity)

Adds the specified entity to the end of this collection.

func append&lt;S>(contentsOf: S)

Adds the specified list of entity as children to this entity.

func insert(Entity, beforeIndex: Int)

Adds the specified entity to this collection directly before the entity at the given index. If the entity is already located before the index, the collection will not change.

func insert&lt;S>(contentsOf: S, beforeIndex: Int)

Adds the specified sequence of entities to this collection in order, directly before the entity at the given index.

func remove(Entity)

Removes the specified child from this entity.

func remove(at: Int)

Removes the specified child from this entity.

func removeAll()

Removes all children from this entity.

func removeAll(where: (Entity) throws -> Bool) rethrows

Removes all entities from this collection that satisfy the given predicate.

func replaceAll&lt;S>(S)

Removes all children from this entity and adds the specified list of entities as the new children.

