

- TabularData
- DataFrameProtocol
-  grouped(by:timeUnit:) 

Instance Method

# grouped(by:timeUnit:)

Creates a grouping of rows that the method selects by choosing unique units of time in a date column you select by column identifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func grouped(
    by columnID: ColumnID,
    timeUnit: Calendar.Component
) -> RowGrouping
```

## Parameters 

`columnID`  

A column identifier.

`timeUnit`  

A component of a calendar date.

## Return Value

A collection of groups.

## Discussion

After the method aggregates the groups, it creates a column with the same name as the original column plus the `timeUnit` name.

## See Also

### Creating a Row Grouping by a Column

func grouped&lt;GroupingKey>(by: ColumnID&lt;GroupingKey>) -> RowGrouping&lt;GroupingKey>

Creates a grouping of rows that the method selects by choosing unique values in a column.

func grouped(by: String, timeUnit: Calendar.Component) -> RowGrouping&lt;Int>

Creates a grouping of rows that the method selects by choosing unique units of time in a date column you select by name.

func grouped&lt;InputKey, GroupingKey>(by: String, transform: (InputKey?) -> GroupingKey?) -> RowGrouping&lt;GroupingKey>

Creates a grouping of rows that the method selects by choosing unique values the transform closure creates with elements of a column you select by name.

func grouped&lt;InputKey, GroupingKey>(by: ColumnID&lt;InputKey>, transform: (InputKey?) -> GroupingKey?) -> RowGrouping&lt;GroupingKey>

Creates a grouping of rows that the method selects by choosing unique values the transform closure creates with elements of a column you select by column identifier.

