

- TabularData
- DataFrameProtocol
-  grouped(by:) 

Instance Method

# grouped(by:)

Creates a grouping from multiple columns that you select by column identifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func grouped(by columnIDs: ColumnID...) -> some RowGroupingProtocol where T : Hashable
```

## Parameters 

`columnIDs`  

A comma-separated, or variadic, list of column identifiers.

## See Also

### Creating a Row Grouping by Multiple Columns

func grouped(by: String...) -> some RowGroupingProtocol

Creates a grouping from multiple columns you select by name.

func grouped&lt;T0, T1>(by: ColumnID&lt;T0>, ColumnID&lt;T1>) -> some RowGroupingProtocol

Creates a grouping from two columns of different types.

func grouped&lt;T0, T1, T2>(by: ColumnID&lt;T0>, ColumnID&lt;T1>, ColumnID&lt;T2>) -> some RowGroupingProtocol

Creates a grouping from three columns of different types.

