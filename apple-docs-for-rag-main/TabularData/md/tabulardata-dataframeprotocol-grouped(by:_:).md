

- TabularData
- DataFrameProtocol
-  grouped(by:\_:) 

Instance Method

# grouped(by:\_:)

Creates a grouping from two columns of different types.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func grouped(
    by column0: ColumnID,
    _ column1: ColumnID
) -> some RowGroupingProtocol where T0 : Hashable, T1 : Hashable
```

## Parameters 

`column0`  

A column identifier.

`column1`  

A second column identifier.

## See Also

### Creating a Row Grouping by Multiple Columns

func grouped(by: String...) -> some RowGroupingProtocol

Creates a grouping from multiple columns you select by name.

func grouped&lt;T>(by: ColumnID&lt;T>...) -> some RowGroupingProtocol

Creates a grouping from multiple columns that you select by column identifier.

func grouped&lt;T0, T1, T2>(by: ColumnID&lt;T0>, ColumnID&lt;T1>, ColumnID&lt;T2>) -> some RowGroupingProtocol

Creates a grouping from three columns of different types.

