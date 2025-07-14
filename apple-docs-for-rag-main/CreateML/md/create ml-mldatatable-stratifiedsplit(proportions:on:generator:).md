

- Create ML
- MLDataTable
-  stratifiedSplit(proportions:on:generator:) 

Instance Method

# stratifiedSplit(proportions:on:generator:)

Randomly split a MLDataTable into a number partitions while stratifying on a user-define label column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func stratifiedSplit(
    proportions: [Double],
    on column: String,
    generator: inout RNG
) throws -> MLDataTable where RNG : RandomNumberGenerator
```

## Parameters 

`proportions`  

An array of values on \[0,1\] specifying the proprtions in each partition. Automatically normalized to 1.

`column`  

The column in an MLDataTable being stratified on.

`generator`  

User-defined RandomNumberGenerator to use in stratification.

## Return Value

A new MLDataTable with an additional partition column with the index of the partition for each row.

## Discussion

The proportions specified will be applied uniformly to each label being partitioned on.

## See Also

### Splitting a data table

func randomSplitBySequence(proportion: Double, by: String, on: String, seed: Int) -> (MLDataTable, remaining: MLDataTable)

func stratifiedSplit(proportions: [Double], on: String, seed: Int) throws -> MLDataTable

Randomly split a MLDataTable into a number partitions while stratifying on a user-define label column.

func stratifiedSplitBySequence&lt;RNG>(proportions: [Double], by: String, on: String, generator: inout RNG) throws -> MLDataTable

Randomly split a MLDataTable into partitions on a user-define label column, while keeping rows from the same sequence in the original order.

func stratifiedSplitBySequence(proportions: [Double], by: String, on: String, seed: Int) throws -> MLDataTable

Randomly split a MLDataTable into partitions on a user-define label column, while keeping rows from the same sequence in the original order.

