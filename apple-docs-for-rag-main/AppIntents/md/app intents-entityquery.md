

- App Intents
-  EntityQuery 

Protocol

# EntityQuery

An interface for locating entities using their identifiers.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol EntityQuery : DynamicOptionsProvider, PersistentlyIdentifiable, Sendable
```

## Mentioned in 

Integrating custom data types into your intents

## Overview

The entity query provides the model object in which ways instances of a particular app entity type can be queried by Siri and the Shortcuts app, and implements the retrieval of such instances.

### Conform to the EntityQuery Protocol

In order to allow Siri and Shortcuts to retrieve AppEntity instances, create a new type conforming to `EntityQuery`.

### Resolving Entities by identifier

In some scenarios, Siri or Shortcuts already knows exactly which entity the user is referring to, and needs to retrieve the actual entity instance given its unique identifier.

To support this retrieval method, implement entities(for:), which given an array of AppEntity identifiers, returns corresponding entity instances. The method should first lookup if said instance already exists in memory. If the instance doesn’t exist, then `perform` can make asynchronous calls to retrieve the entity (ex: from disk or from a remote back-end). If the entity corresponding to a supplied identifier is not available anymore, then it should be omitted from the returned array.

```
struct MyPhotoQuery: any EntityQuery {
    func entities(for identifiers: [UUID]) async throws -> [MyPhoto] {
        myPhotoStore.filter { ids.contains($0.id) }
    }
```

## Topics

### Creating a query

init()

**Required**

### Searching for entities

func entities(for: [Self.Entity.ID]) async throws -> [Self.Entity]

Retrieves instances by identifier.

**Required** Default implementation provided.

associatedtype Entity : AppEntity = Self.Result.Result.ValueType

The entity type that this query knows how to resolve.

**Required**

### Suggesting entities

func suggestedEntities() async throws -> Self.Result

Returns the initial results shown when a list of options backed by this query is presented.

**Required** Default implementations provided.

### Associated Types

associatedtype Result = [Self.Entity]

**Required**

## Relationships

### Inherits From

- DynamicOptionsProvider
- PersistentlyIdentifiable
- Sendable

### Inherited By

- EntityPropertyQuery
- EntityStringQuery
- EnumerableEntityQuery
- UniqueAppEntityQuery

### Conforming Types

- UniqueAppEntityProvider

## See Also

### Identifier-based queries

protocol EnumerableEntityQuery

An interface you use to provide a short list of entities that are relatively small in size.

