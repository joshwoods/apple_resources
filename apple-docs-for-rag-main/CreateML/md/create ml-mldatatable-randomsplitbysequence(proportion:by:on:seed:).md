

- Create ML
- MLDataTable
-  randomSplitBySequence(proportion:by:on:seed:) 

Instance Method

# randomSplitBySequence(proportion:by:on:seed:)

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
func randomSplitBySequence(
    proportion: Double,
    by sequenceIdentifierColumn: String,
    on column: String,
    seed: Int = 1
) -> (MLDataTable, remaining: MLDataTable)
```

## See Also

### Splitting a data table

func stratifiedSplit&lt;RNG>(proportions: [Double], on: String, generator: inout RNG) throws -> MLDataTable

Randomly split a MLDataTable into a number partitions while stratifying on a user-define label column.

func stratifiedSplit(proportions: [Double], on: String, seed: Int) throws -> MLDataTable

Randomly split a MLDataTable into a number partitions while stratifying on a user-define label column.

func stratifiedSplitBySequence&lt;RNG>(proportions: [Double], by: String, on: String, generator: inout RNG) throws -> MLDataTable

Randomly split a MLDataTable into partitions on a user-define label column, while keeping rows from the same sequence in the original order.

func stratifiedSplitBySequence(proportions: [Double], by: String, on: String, seed: Int) throws -> MLDataTable

Randomly split a MLDataTable into partitions on a user-define label column, while keeping rows from the same sequence in the original order.

