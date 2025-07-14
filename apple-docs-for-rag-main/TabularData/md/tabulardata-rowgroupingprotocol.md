

- TabularData
-  RowGroupingProtocol 

Protocol

# RowGroupingProtocol

A type that represents a collection of row selections that have the same value in a column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol RowGroupingProtocol : CustomStringConvertible
```

## Topics

### Inspecting a Row Grouping

var count: Int

The number of groups in the row grouping.

**Required**

### Transforming a Row Grouping

func mapGroups((DataFrame.Slice) throws -> DataFrame) rethrows -> Self

Generates a row grouping that applies a transformation closure to each group in the original.

**Required**

### Splitting a Row Grouping

func randomSplit(by: Double) -> (Self, Self)

Generates two row groupings by randomly splitting the original with a proportion.

func randomSplit(by: Double, seed: Int?) -> (Self, Self)

Generates two row groupings by randomly splitting the original by a proportion.

**Required**

### Aggregating a Row Grouping

func counts() -> DataFrame

Generates a data frame with two columns, one that has a row for each group key and another for the number of rows in the group.

func counts(order: Order?) -> DataFrame

Generates a data frame, that you choose how to sort, with two columns, one that has a row for each group key and another for the number or rows in the group.

**Required**

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

Generates a data frame by aggregating each group’s contents for each column you select by name.

**Required** Default implementation provided.

### Flattening a Row Grouping

func ungrouped() -> DataFrame

Generates a data frame that contains all the rows from each group in the row grouping.

**Required**

### Summarizing a Row Grouping

func summary() -> any GroupSummaries

Generates a group summaries instance of the row grouping’s columns.

**Required**

func summary(of: [String]) -> any GroupSummaries

Generates a group summaries instance of the row grouping’s columns you select by name.

**Required** Default implementation provided.

protocol GroupSummaries

A collection of group summaries.

### Instance Methods

func filter((DataFrame.Slice) throws -> Bool) rethrows -> Self

Returns a row grouping containing only the groups that satisfy a predicate.

**Required**

func quantiles&lt;N>(String, N.Type, quantile: N, order: Order?) -> DataFrame

Generates a data frame that contains the quantile of each group’s rows along a column you select by name.

func quantiles&lt;N>(ColumnID&lt;N>, quantile: N, order: Order?) -> DataFrame

Generates a data frame that contains the quantiles of each group’s rows along a column you select by column identifier.

### Subscripts

subscript(Any?...) -> DataFrame.Slice?

Retrieves a group slice by key.

**Required**

## Relationships

### Inherits From

- CustomStringConvertible

### Conforming Types

- RowGrouping

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

struct RowGrouping

A collection of row selections that have the same value in a column.

func grouped(by: String) -> any RowGroupingProtocol

Creates a grouping of rows that the method selects by choosing unique values in a column.

func grouped&lt;T0, T1>(by: ColumnID&lt;T0>, ColumnID&lt;T1>) -> some RowGroupingProtocol

Creates a grouping from two columns of different types.

func grouped&lt;T0, T1, T2>(by: ColumnID&lt;T0>, ColumnID&lt;T1>, ColumnID&lt;T2>) -> some RowGroupingProtocol

Creates a grouping from three columns of different types.

