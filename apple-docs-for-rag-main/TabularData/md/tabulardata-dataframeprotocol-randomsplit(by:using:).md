

- TabularData
- DataFrameProtocol
-  randomSplit(by:using:) 

Instance Method

# randomSplit(by:using:)

Generates two data frame slices by randomly splitting the rows of the data table type with a random-number generator.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func randomSplit(
    by proportion: Double,
    using generator: inout G
) -> (DataFrame.Slice, DataFrame.Slice) where G : RandomNumberGenerator
```

## Parameters 

`proportion`  

A proportion in the range `[0.0, 1.0]`.

`generator`  

A random-number generator.

## Return Value

A tuple of two data frame slices.

## See Also

### Creating Two Slices by Splitting Rows

func randomSplit(by: Double, seed: Int?) -> (DataFrame.Slice, DataFrame.Slice)

Generates two data frame slices by randomly splitting the rows of the data table.

