

- App Intents
- EntityPropertyQuery
-  entities(matching:mode:sortedBy:limit:) 

Instance Method

# entities(matching:mode:sortedBy:limit:)

Retrieves instances matching the supplied comparators.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func entities(
    matching comparators: [Self.ComparatorMappingType],
    mode: Self.ComparatorMode,
    sortedBy: [EntityQuerySort],
    limit: Int?
) async throws -> Self.Result
```

**Required**

## Parameters 

`comparators`  

Array containing mapped values for comparators that entities need to match

`mode`  

Whether entity instances should match any or all comparators

`sortedBy`  

Array describing the query’s sorting order

`limit`  

Optional limit on the number of entity instances to return

## See Also

### Searching for entities

typealias Sort

typealias ComparatorMode

enum EntityQueryComparatorMode

Modes that determine how to apply a query’s comparators.

