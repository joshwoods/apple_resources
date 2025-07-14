

- RealityKit
- Views and attachments
- RealityViewEntityCollection
-  EntityCollection Implementations 

API Collection

# EntityCollection Implementations

## Topics

### Instance Methods

func append(Entity)

Adds the specified entity to the end of this collection.

func append&lt;S>(contentsOf: S)

Adds the specified sequence of entities to the end of this collection, in order.

func insert(Entity, beforeIndex: Int)

Adds the specified entity to this collection directly before the entity at the given index. If the entity is already located before the index, the collection will not change.

func remove(Entity)

Removes the entity from the collection.

func removeAll()

Removes all entities from this collection.

func removeAll(where: (Entity) throws -> Bool) rethrows

Removes all entities from this collection that satisfy the given predicate.

func replaceAll&lt;S>(S)

Replaces all entities in this collection with those from the given sequence.

