

- TabularData
- DataFrame
-  stratifiedSplit(on:by:randomSeed:) 

Instance Method

# stratifiedSplit(on:by:randomSeed:)

Generates two data frames by randomly splitting the rows of a column, which you select by column identifier, into strata.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func stratifiedSplit(
    on columnID: ColumnID,
    by proportion: Double,
    randomSeed: Int? = nil
) -> (DataFrame, DataFrame) where T : Hashable
```

## Parameters 

`columnID`  

A column identifier.

`proportion`  

A proportion in the range `[0.0, 1.0]`.

`randomSeed`  

A seed number for a random-number generator.

## Return Value

A tuple of two data frames.

