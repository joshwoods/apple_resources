

- TabularData
- RowGrouping
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Retrieves a group at an index.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(position: Int) -> (key: GroupingKey?, group: DataFrame.Slice) { get }
```

Available when `GroupingKey` conforms to `Hashable`.

## Parameters 

`position`  

A valid index to a group in the row grouping.

## See Also

### Inspecting a Row Grouping

var count: Int

The number of groups in the row grouping.

