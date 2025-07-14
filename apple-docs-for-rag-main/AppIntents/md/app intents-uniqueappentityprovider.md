

- App Intents
-  UniqueAppEntityProvider 

Structure

# UniqueAppEntityProvider

A simplified query type conforming to `UniqueAppEntityQuery`. Use this as the value of the `defaultQuery` of an entity conforming to `UniqueAppEntity`.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct UniqueAppEntityProvider where Entity : UniqueAppEntity
```

## Topics

### Initializers

init()

init(() async throws -> Entity)

### Instance Methods

func uniqueEntity() async throws -> Entity

### Type Aliases

typealias DefaultValue

typealias Result

typealias Unique

### Default Implementations

DynamicOptionsProvider Implementations

EntityQuery Implementations

EnumerableEntityQuery Implementations

PersistentlyIdentifiable Implementations

UniqueAppEntityQuery Implementations

## Relationships

### Conforms To

- DynamicOptionsProvider
- EntityQuery
- EnumerableEntityQuery
- PersistentlyIdentifiable
- Sendable
- UniqueAppEntityQuery

## See Also

### Unique entity queries

protocol UniqueAppEntityQuery

A query designed for only returning a single possible value, provided by `uniqueEntity`. Protocol extensions will provide the other required query methods based on that.

