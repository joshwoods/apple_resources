

- TabularData
- DataFrame
- DataFrame.Slice
-  grouped(by:transform:) 

Instance Method

# grouped(by:transform:)

Creates a grouping of rows that the method selects by choosing unique values the transform closure creates with elements of a column you select by column identifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func grouped(
    by columnID: ColumnID,
    transform: (InputKey?) -> GroupingKey?
) -> RowGrouping where GroupingKey : Hashable
```

## Parameters 

`columnID`  

A column identifier.

`transform`  

A closure that transforms a column’s elements into a hashable type.

## Return Value

A collection of groups.

## Discussion

Create groupings that group rows by:

- Telephone area codes

- The first letter of a person’s last name

- A date’s year or quarter

- Number ranges

## See Also

### Grouping Rows

func grouped(by: String, timeUnit: Calendar.Component) -> RowGrouping&lt;Int>

Creates a grouping of rows that the method selects by choosing unique units of time in a date column you select by name.

func grouped(by: ColumnID&lt;Date>, timeUnit: Calendar.Component) -> RowGrouping&lt;Int>

Creates a grouping of rows that the method selects by choosing unique units of time in a date column you select by column identifier.

func grouped&lt;InputKey, GroupingKey>(by: String, transform: (InputKey?) -> GroupingKey?) -> RowGrouping&lt;GroupingKey>

Creates a grouping of rows that the method selects by choosing unique values the transform closure creates with elements of a column you select by name.

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

