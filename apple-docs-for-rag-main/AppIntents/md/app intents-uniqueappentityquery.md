

- App Intents
-  UniqueAppEntityQuery 

Protocol

# UniqueAppEntityQuery

A query designed for only returning a single possible value, provided by `uniqueEntity`. Protocol extensions will provide the other required query methods based on that.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
protocol UniqueAppEntityQuery : EnumerableEntityQuery where Self.Entity : UniqueAppEntity
```

## Topics

### Associated Types

associatedtype Unique

**Required**

### Instance Methods

func uniqueEntity() async throws -> Self.Unique

**Required**

## Relationships

### Inherits From

- DynamicOptionsProvider
- EntityQuery
- EnumerableEntityQuery
- PersistentlyIdentifiable
- Sendable

### Conforming Types

- UniqueAppEntityProvider

## See Also

### Unique entity queries

struct UniqueAppEntityProvider

A simplified query type conforming to `UniqueAppEntityQuery`. Use this as the value of the `defaultQuery` of an entity conforming to `UniqueAppEntity`.

