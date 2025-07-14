

- App Intents
- EntityPropertyQuery
-  EntityPropertyQuery.ComparatorMode 

Type Alias

# EntityPropertyQuery.ComparatorMode

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
typealias ComparatorMode = EntityQueryComparatorMode
```

## See Also

### Searching for entities

func entities(matching: [Self.ComparatorMappingType], mode: Self.ComparatorMode, sortedBy: [EntityQuerySort&lt;Self.Entity>], limit: Int?) async throws -> Self.Result

Retrieves instances matching the supplied comparators.

**Required**

typealias Sort

enum EntityQueryComparatorMode

Modes that determine how to apply a query’s comparators.

