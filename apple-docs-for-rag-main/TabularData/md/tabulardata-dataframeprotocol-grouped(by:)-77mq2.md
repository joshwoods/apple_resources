

- TabularData
- DataFrameProtocol
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

## See Also

### Creating a Row Grouping by a Column

func grouped(by: String, timeUnit: Calendar.Component) -> RowGrouping&lt;Int>

Creates a grouping of rows that the method selects by choosing unique units of time in a date column you select by name.

func grouped(by: ColumnID&lt;Date>, timeUnit: Calendar.Component) -> RowGrouping&lt;Int>

Creates a grouping of rows that the method selects by choosing unique units of time in a date column you select by column identifier.

func grouped&lt;InputKey, GroupingKey>(by: String, transform: (InputKey?) -> GroupingKey?) -> RowGrouping&lt;GroupingKey>

Creates a grouping of rows that the method selects by choosing unique values the transform closure creates with elements of a column you select by name.

func grouped&lt;InputKey, GroupingKey>(by: ColumnID&lt;InputKey>, transform: (InputKey?) -> GroupingKey?) -> RowGrouping&lt;GroupingKey>

Creates a grouping of rows that the method selects by choosing unique values the transform closure creates with elements of a column you select by column identifier.

