

- TabularData
- RowGrouping
-  mapGroups(\_:) 

Instance Method

# mapGroups(\_:)

Generates a row grouping that applies a transformation closure to each group in the original.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func mapGroups(_ transform: (DataFrame.Slice) throws -> DataFrame) rethrows -> RowGrouping
```

## Parameters 

`transform`  

A closure that generates a data frame from a data frame slice that represents a group.

