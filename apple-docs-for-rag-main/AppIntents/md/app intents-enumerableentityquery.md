

- App Intents
-  EnumerableEntityQuery 

Protocol

# EnumerableEntityQuery

An interface you use to provide a short list of entities that are relatively small in size.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
protocol EnumerableEntityQuery : EntityQuery
```

## Mentioned in 

Integrating custom data types into your intents

## Overview

By implementing an `EnumerableEntityQuery`, you enable the Shortcuts app to generate a Find action and do filtering automatically. Use it in cases where the count of entities is relatively small, and their size in memory is limited. For situations where there may be many thousands of entities, or where individual entities may become large in memory usage, use EntityPropertyQuery to allow better performance by fetching only the entities matching the criteria from your model.

## Topics

### Instance Methods

func allEntities() async throws -> Self.Result

Returns all available results.

**Required** Default implementation provided.

### Type Properties

static var findIntentDescription: IntentDescription?

Defines how the generated ‘Find’ Shortcuts action of this query type is displayed to the user.

**Required** Default implementation provided.

## Relationships

### Inherits From

- DynamicOptionsProvider
- EntityQuery
- PersistentlyIdentifiable
- Sendable

### Inherited By

- UniqueAppEntityQuery

### Conforming Types

- UniqueAppEntityProvider

## See Also

### Identifier-based queries

protocol EntityQuery

An interface for locating entities using their identifiers.

