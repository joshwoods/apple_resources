

- TabularData
- DataFrame
-  grouped(by:timeUnit:) 

Instance Method

# grouped(by:timeUnit:)

Creates a grouping of rows that the method selects by choosing unique units of time in a date column you select by name.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func grouped(
    by columnName: String,
    timeUnit: Calendar.Component
) -> RowGrouping
```

## Parameters 

`columnName`  

The name of a column.

`timeUnit`  

A component of a calendar date.

## Return Value

A collection of groups.

## Discussion

After the method aggregates the groups, it creates a column with the same name as the original column plus the `timeUnit` name.

## See Also

### Grouping Rows

func grouped(by: ColumnID&lt;Date>, timeUnit: Calendar.Component) -> RowGrouping&lt;Int>

Creates a grouping of rows that the method selects by choosing unique units of time in a date column you select by column identifier.

func grouped&lt;InputKey, GroupingKey>(by: String, transform: (InputKey?) -> GroupingKey?) -> RowGrouping&lt;GroupingKey>

Creates a grouping of rows that the method selects by choosing unique values the transform closure creates with elements of a column you select by name.

func grouped&lt;InputKey, GroupingKey>(by: ColumnID&lt;InputKey>, transform: (InputKey?) -> GroupingKey?) -> RowGrouping&lt;GroupingKey>

Creates a grouping of rows that the method selects by choosing unique values the transform closure creates with elements of a column you select by column identifier.

struct RowGrouping

A collection of row selections that have the same value in a column.

func grouped(by: String) -> any RowGroupingProtocol

Creates a grouping of rows that the method selects by choosing unique values in a column.

func grouped&lt;T0, T1>(by: ColumnID&lt;T0>, ColumnID&lt;T1>) -> some RowGroupingProtocol

Creates a grouping from two columns of different types.

func grouped&lt;T0, T1, T2>(by: ColumnID&lt;T0>, ColumnID&lt;T1>, ColumnID&lt;T2>) -> some RowGroupingProtocol

Creates a grouping from three columns of different types.

protocol RowGroupingProtocol

A type that represents a collection of row selections that have the same value in a column.

