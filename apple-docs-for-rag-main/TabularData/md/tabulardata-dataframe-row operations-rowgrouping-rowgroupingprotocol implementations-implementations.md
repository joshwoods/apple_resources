

- TabularData
- DataFrame
- Row Operations
- RowGrouping
-  RowGroupingProtocol Implementations 

API Collection

# RowGroupingProtocol Implementations

## Topics

### Instance Methods

func aggregated&lt;Element, Result>(on: ColumnID&lt;Element>, into: String?, transform: (DiscontiguousColumnSlice&lt;Element>) throws -> Result) rethrows -> DataFrame

Generates a data frame with a column for the group identifier and a column of values from the transform.

func aggregated&lt;Element, Result>(on: String..., naming: (String) -> String, transform: (DiscontiguousColumnSlice&lt;Element>) throws -> Result?) rethrows -> DataFrame

Generates a data frame by aggregating each group’s contents for each column you select by name.

func counts() -> DataFrame

Generates a data frame with two columns, one that has a row for each group key and another for the number of rows in the group.

func maximums&lt;N>(String, N.Type, order: Order?) -> DataFrame

Generates a data frame that contains the maximums of each group’s rows along a column you select by name.

func maximums&lt;N>(ColumnID&lt;N>, order: Order?) -> DataFrame

Generates a data frame that contains the maximums of each group’s rows along a column you select by column identifier.

func means&lt;N>(String, N.Type, order: Order?) -> DataFrame

Generates a data frame that contains the average mean of each group’s rows along a column you select by name.

func means&lt;N>(ColumnID&lt;N>, order: Order?) -> DataFrame

Generates a data frame that contains the average mean of each group’s rows along a column you select by column identifier.

func minimums&lt;N>(String, N.Type, order: Order?) -> DataFrame

Generates a data frame that contains the minimums of each group’s rows along a column you select by name.

func minimums&lt;N>(ColumnID&lt;N>, order: Order?) -> DataFrame

Generates a data frame that contains the minimums of each group’s rows along a column you select by column identifier.

func quantiles&lt;N>(String, N.Type, quantile: N, order: Order?) -> DataFrame

Generates a data frame that contains the quantile of each group’s rows along a column you select by name.

func quantiles&lt;N>(ColumnID&lt;N>, quantile: N, order: Order?) -> DataFrame

Generates a data frame that contains the quantiles of each group’s rows along a column you select by column identifier.

func randomSplit(by: Double) -> (Self, Self)

Generates two row groupings by randomly splitting the original with a proportion.

func randomSplit(by: Double, seed: Int?) -> (RowGrouping&lt;GroupingKey>, RowGrouping&lt;GroupingKey>)

Generates two row groupings by randomly splitting the original with a proportion and a seed number.

func summary() -> any GroupSummaries

Generates a group summaries instance for the columns of the row grouping.

func summary(of: [String]) -> any GroupSummaries

Generates a group summaries instance for the columns you select by name.

func sums&lt;N>(String, N.Type, order: Order?) -> DataFrame

Generates a data frame that contains the sum of each group’s rows along a column you select by name.

func sums&lt;N>(ColumnID&lt;N>, order: Order?) -> DataFrame

Generates a data frame that contains the sum of each group’s rows along a column you select by column identifier.

