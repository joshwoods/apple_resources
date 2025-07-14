

- RealityKit
-  EntityCollection 

Protocol

# EntityCollection

An ordered, mutable collection of entities.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
protocol EntityCollection : Collection where Self.Element == Entity, Self.Index == Int
```

## Topics

### Instance Methods

func append(Entity)

Adds the specified entity to the end of this collection.

**Required** Default implementation provided.

func append&lt;S>(contentsOf: S)

Adds the specified sequence of entities to the end of this collection, in order.

**Required** Default implementation provided.

func insert(Entity, beforeIndex: Int)

Adds the specified entity to this collection directly before the entity at the given index. If the entity is already located before the index, the collection will not change.

**Required** Default implementation provided.

func insert&lt;S>(contentsOf: S, beforeIndex: Int)

Adds the specified sequence of entities to this collection in order, directly before the entity at the given index.

**Required**

func remove(Entity)

Removes the entity from the collection.

**Required** Default implementation provided.

func remove(at: Int)

Removes the entity at the given index from this collection.

**Required**

func removeAll()

Removes all entities from this collection.

**Required** Default implementation provided.

func removeAll(where: (Entity) throws -> Bool) rethrows

Removes all entities from this collection that satisfy the given predicate.

**Required** Default implementation provided.

func replaceAll&lt;S>(S)

Replaces all entities in this collection with those from the given sequence.

**Required** Default implementation provided.

## Relationships

### Inherits From

- Collection
- Sequence

### Conforming Types

- Entity.ChildCollection
- RealityRenderer.EntityCollection
- RealityViewEntityCollection

## See Also

### SwiftUI scene presentation

struct RealityView

A view that contains RealityKit content.

struct RealityViewContent

The content of a visionOS reality view.

struct RealityViewCameraContent

The content of a reality view that is displayed through a camera.

protocol RealityViewContentProtocol

A protocol representing the content of a reality view.

struct RealityViewDefaultPlaceholder

A view that represents the default placeholder for a RealityView.

struct RealityViewEntityCollection

A collection of entities in a RealityView.

