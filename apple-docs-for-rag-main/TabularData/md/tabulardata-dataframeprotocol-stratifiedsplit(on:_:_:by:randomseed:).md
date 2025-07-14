

- TabularData
- DataFrameProtocol
-  stratifiedSplit(on:\_:\_:by:randomSeed:) 

Instance Method

# stratifiedSplit(on:\_:\_:by:randomSeed:)

Generates two data frames by randomly splitting the rows of three columns, which you select by column identifiers, into strata.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func stratifiedSplit(
    on columnID0: ColumnID,
    _ columnID1: ColumnID,
    _ columnID2: ColumnID,
    by proportion: Double,
    randomSeed: Int? = nil
) -> (DataFrame, DataFrame) where T0 : Hashable, T1 : Hashable, T2 : Hashable
```

## Parameters 

`columnID0`  

A column identifier.

`columnID1`  

A second column identifier.

`columnID2`  

A third column identifier.

`proportion`  

A proportion in the range `[0.0, 1.0]`.

`randomSeed`  

A seed number for a random-number generator.

## Return Value

A tuple of two data frames.

## See Also

### Creating Two Data Frames by Splitting Rows

func stratifiedSplit(on: String, by: Double, randomSeed: Int?) -> (DataFrame, DataFrame)

Generates two data frames by randomly splitting the rows of a column, which you select by its name, into strata.

func stratifiedSplit(on: String..., by: Double, randomSeed: Int?) -> (DataFrame, DataFrame)

Generates two data frames by randomly splitting the rows of multiple columns, which you select by their names, into strata.

func stratifiedSplit&lt;T>(on: ColumnID&lt;T>, by: Double, randomSeed: Int?) -> (DataFrame, DataFrame)

Generates two data frames by randomly splitting the rows of a column, which you select by column identifier, into strata.

func stratifiedSplit&lt;T0, T1>(on: ColumnID&lt;T0>, ColumnID&lt;T1>, by: Double, randomSeed: Int?) -> (DataFrame, DataFrame)

Generates two data frames by randomly splitting the rows of two columns, which you select by column identifiers, into strata.

