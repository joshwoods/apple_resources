

- App Intents
- EntityQuery
-  Entity 

Associated Type

# Entity

The entity type that this query knows how to resolve.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
associatedtype Entity : AppEntity = Self.Result.Result.ValueType where Self.Entity == Self.Result.Result
```

**Required**

## See Also

### Searching for entities

func entities(for: [Self.Entity.ID]) async throws -> [Self.Entity]

Retrieves instances by identifier.

**Required** Default implementation provided.

