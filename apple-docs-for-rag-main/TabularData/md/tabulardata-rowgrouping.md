

- TabularData
-  RowGrouping 

Structure

# RowGrouping

A collection of row selections that have the same value in a column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct RowGrouping where GroupingKey : Hashable
```

## Topics

### Creating a Row Grouping

init&lt;D>(frame: D, columnName: String, timeUnit: Calendar.Component)

Creates a row grouping from a column with date or time elements.

init&lt;D>(groups: [(GroupingKey?, D)], groupKeysColumnName: String)

Creates a row grouping from a list of groups.

### Inspecting a Row Grouping

var count: Int

The number of groups in the row grouping.

subscript(Int) -> (key: GroupingKey?, group: DataFrame.Slice)

Retrieves a group at an index.

### Transforming a Row Grouping

func mapGroups((DataFrame.Slice) throws -> DataFrame) rethrows -> RowGrouping&lt;GroupingKey>

Generates a row grouping that applies a transformation closure to each group in the original.

### Splitting a Row Grouping

func randomSplit(by: Double) -> (Self, Self)

Generates two row groupings by randomly splitting the original with a proportion.

func randomSplit(by: Double, seed: Int?) -> (RowGrouping&lt;GroupingKey>, RowGrouping&lt;GroupingKey>)

Generates two row groupings by randomly splitting the original with a proportion and a seed number.

### Aggregating a Row Grouping

func counts() -> DataFrame

Generates a data frame with two columns, one that has a row for each group key and another for the number of rows in the group.

func counts(order: Order?) -> DataFrame

Generates a data frame with two columns, one that has a row for each group key and another for the number of rows in the group.

func sums&lt;N>(String, N.Type, order: Order?) -> DataFrame

Generates a data frame that contains the sum of each group’s rows along a column you select by name.

func sums&lt;N>(ColumnID&lt;N>, order: Order?) -> DataFrame

Generates a data frame that contains the sum of each group’s rows along a column you select by column identifier.

func means&lt;N>(String, N.Type, order: Order?) -> DataFrame

Generates a data frame that contains the average mean of each group’s rows along a column you select by name.

func means&lt;N>(ColumnID&lt;N>, order: Order?) -> DataFrame

Generates a data frame that contains the average mean of each group’s rows along a column you select by column identifier.

func minimums&lt;N>(String, N.Type, order: Order?) -> DataFrame

Generates a data frame that contains the minimums of each group’s rows along a column you select by name.

func minimums&lt;N>(ColumnID&lt;N>, order: Order?) -> DataFrame

Generates a data frame that contains the minimums of each group’s rows along a column you select by column identifier.

func maximums&lt;N>(String, N.Type, order: Order?) -> DataFrame

Generates a data frame that contains the maximums of each group’s rows along a column you select by name.

func maximums&lt;N>(ColumnID&lt;N>, order: Order?) -> DataFrame

Generates a data frame that contains the maximums of each group’s rows along a column you select by column identifier.

func aggregated&lt;Element, Result>(on: ColumnID&lt;Element>, into: String?, transform: (DiscontiguousColumnSlice&lt;Element>) throws -> Result) rethrows -> DataFrame

Generates a data frame with a column for the group identifier and a column of values from the transform.

func aggregated&lt;Element, Result>(on: [String], naming: (String) -> String, transform: (DiscontiguousColumnSlice&lt;Element>) throws -> Result?) rethrows -> DataFrame

Generates a data frame by aggregating each group’s contents for each column you list by name.

func aggregated&lt;Element, Result>(on: String..., naming: (String) -> String, transform: (DiscontiguousColumnSlice&lt;Element>) throws -> Result?) rethrows -> DataFrame

Generates a data frame by aggregating each group’s contents for each column you select by name.

### Flattening a Row Grouping

func ungrouped() -> DataFrame

Generates a data frame that contains all the rows from each group in the row grouping.

### Summarizing a Row Grouping

func summary() -> any GroupSummaries

Generates a group summaries instance for the columns of the row grouping.

func summary(of: [String]) -> any GroupSummaries

Generates a group summaries instance for the columns you select by name.

protocol GroupSummaries

A collection of group summaries.

### Describing a Row Grouping

var description: String

A text representation of the row grouping.

### Subscripts

subscript(Any?...) -> DataFrame.Slice?

Retrieves a group slice by key.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

RandomAccessCollection Implementations

RowGroupingProtocol Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Copyable
- CustomStringConvertible
- RandomAccessCollection
- RowGroupingProtocol
- Sequence

## See Also

### Grouping Rows

func grouped(by: String, timeUnit: Calendar.Component) -> RowGrouping&lt;Int>

Creates a grouping of rows that the method selects by choosing unique units of time in a date column you select by name.

func grouped(by: ColumnID&lt;Date>, timeUnit: Calendar.Component) -> RowGrouping&lt;Int>

Creates a grouping of rows that the method selects by choosing unique units of time in a date column you select by column identifier.

func grouped&lt;InputKey, GroupingKey>(by: String, transform: (InputKey?) -> GroupingKey?) -> RowGrouping&lt;GroupingKey>

Creates a grouping of rows that the method selects by choosing unique values the transform closure creates with elements of a column you select by name.

func grouped&lt;InputKey, GroupingKey>(by: ColumnID&lt;InputKey>, transform: (InputKey?) -> GroupingKey?) -> RowGrouping&lt;GroupingKey>

Creates a grouping of rows that the method selects by choosing unique values the transform closure creates with elements of a column you select by column identifier.

func grouped(by: String) -> any RowGroupingProtocol

Creates a grouping of rows that the method selects by choosing unique values in a column.

func grouped&lt;T0, T1>(by: ColumnID&lt;T0>, ColumnID&lt;T1>) -> some RowGroupingProtocol

Creates a grouping from two columns of different types.

func grouped&lt;T0, T1, T2>(by: ColumnID&lt;T0>, ColumnID&lt;T1>, ColumnID&lt;T2>) -> some RowGroupingProtocol

Creates a grouping from three columns of different types.

protocol RowGroupingProtocol

A type that represents a collection of row selections that have the same value in a column.

