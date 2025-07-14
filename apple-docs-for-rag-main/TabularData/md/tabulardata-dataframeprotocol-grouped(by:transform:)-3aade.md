

- TabularData
- DataFrameProtocol
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

### Creating a Row Grouping by a Column

func grouped&lt;GroupingKey>(by: ColumnID&lt;GroupingKey>) -> RowGrouping&lt;GroupingKey>

Creates a grouping of rows that the method selects by choosing unique values in a column.

func grouped(by: String, timeUnit: Calendar.Component) -> RowGrouping&lt;Int>

Creates a grouping of rows that the method selects by choosing unique units of time in a date column you select by name.

func grouped(by: ColumnID&lt;Date>, timeUnit: Calendar.Component) -> RowGrouping&lt;Int>

Creates a grouping of rows that the method selects by choosing unique units of time in a date column you select by column identifier.

func grouped&lt;InputKey, GroupingKey>(by: String, transform: (InputKey?) -> GroupingKey?) -> RowGrouping&lt;GroupingKey>

Creates a grouping of rows that the method selects by choosing unique values the transform closure creates with elements of a column you select by name.

