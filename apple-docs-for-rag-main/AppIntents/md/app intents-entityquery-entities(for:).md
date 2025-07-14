

- App Intents
- EntityQuery
-  entities(for:) 

Instance Method

# entities(for:)

Retrieves instances by identifier.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func entities(for identifiers: [Self.Entity.ID]) async throws -> [Self.Entity]
```

**Required** Default implementation provided.

## Parameters 

`identifiers`  

Array of entity identifiers

## Mentioned in 

Integrating custom data types into your intents

## Discussion

Identifiers for which there is no matching entity are skipped, so the number of elements in the resulting array of entities can be smaller than the number of supplied identifiers.

## Default Implementations

### EntityQuery Implementations

func entities(for: [Self.Unique.ID]) async throws -> [Self.Unique]

## See Also

### Searching for entities

associatedtype Entity : AppEntity = Self.Result.Result.ValueType

The entity type that this query knows how to resolve.

**Required**

