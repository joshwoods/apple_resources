

- Create ML
- MLDataTable
-  group(columnsNamed:aggregators:) 

Instance Method

# group(columnsNamed:aggregators:)

Creates a new data table with the given columns and adds a new column for each of the given aggregators.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func group(
    columnsNamed: String...,
    aggregators: S
) -> MLDataTable where S : Sequence, S.Element == MLDataTable.Aggregator
```

## Return Value

A new data table.

## Discussion

- columnsNamed: The name of the columns to include in the new data table.

- aggregators: A sequence of aggregators, each of which adds a column in the new data table.

## See Also

### Aggregating Rows

struct Aggregator

A collection of column operations you can use with a data table’s `group` method.

