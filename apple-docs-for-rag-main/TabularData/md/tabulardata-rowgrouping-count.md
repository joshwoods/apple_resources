

- TabularData
- RowGrouping
-  count 

Instance Property

# count

The number of groups in the row grouping.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var count: Int { get }
```

Available when `GroupingKey` conforms to `Hashable`.

## See Also

### Inspecting a Row Grouping

subscript(Int) -> (key: GroupingKey?, group: DataFrame.Slice)

Retrieves a group at an index.

