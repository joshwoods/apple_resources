

- TabularData
- RowGroupingProtocol
-  maximums(\_:\_:order:) 

Instance Method

# maximums(\_:\_:order:)

Generates a data frame that contains the maximums of each group’s rows along a column you select by name.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func maximums(
    _ columnName: String,
    _ type: N.Type,
    order: Order? = nil
) -> DataFrame where N : Comparable
```

## Parameters 

`columnName`  

The name of a column.

`type`  

The type of the column.

`order`  

A sorting order the method uses to sort the data frame by its maximum column.

## See Also

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

func maximums&lt;N>(ColumnID&lt;N>, order: Order?) -> DataFrame

Generates a data frame that contains the maximums of each group’s rows along a column you select by column identifier.

func aggregated&lt;Element, Result>(on: ColumnID&lt;Element>, into: String?, transform: (DiscontiguousColumnSlice&lt;Element>) throws -> Result) rethrows -> DataFrame

Generates a data frame with a column for the group identifier and a column of values from the transform.

func aggregated&lt;Element, Result>(on: [String], naming: (String) -> String, transform: (DiscontiguousColumnSlice&lt;Element>) throws -> Result?) rethrows -> DataFrame

Generates a data frame by aggregating each group’s contents for each column you select by name.

**Required** Default implementation provided.

