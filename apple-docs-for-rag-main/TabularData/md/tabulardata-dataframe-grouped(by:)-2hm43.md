

- TabularData
- DataFrame
-  grouped(by:) 

Instance Method

# grouped(by:)

Creates a grouping of rows that the method selects by choosing unique values in a column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func grouped(by columnID: ColumnID) -> RowGrouping where GroupingKey : Hashable
```

## Parameters 

`columnID`  

A column identifier.

## Return Value

A collection of groups.

