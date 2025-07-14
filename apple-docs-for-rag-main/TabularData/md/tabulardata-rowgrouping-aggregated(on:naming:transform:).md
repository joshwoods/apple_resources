

- TabularData
- RowGrouping
-  aggregated(on:naming:transform:) 

Instance Method

# aggregated(on:naming:transform:)

Generates a data frame by aggregating each group’s contents for each column you list by name.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func aggregated(
    on columnNames: [String],
    naming: (String) -> String,
    transform: (DiscontiguousColumnSlice) throws -> Result?
) rethrows -> DataFrame
```

## Parameters 

`columnNames`  

A comma-separated, or variadic, list of column names.

`naming`  

A closure that converts a column name to another name.

`transform`  

A closure that aggregates a group’s elements in a specific column.

## Discussion

The data frame contains two columns that:

- Identify each group

- Store the results of your aggregation transform closure

## See Also

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

func aggregated&lt;Element, Result>(on: String..., naming: (String) -> String, transform: (DiscontiguousColumnSlice&lt;Element>) throws -> Result?) rethrows -> DataFrame

Generates a data frame by aggregating each group’s contents for each column you select by name.

