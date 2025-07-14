

- TabularData
- DataFrame
- DataFrame.Slice
-  randomSplit(by:seed:) 

Instance Method

# randomSplit(by:seed:)

Generates two data frame slices by randomly splitting the rows of the data table.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func randomSplit(
    by proportion: Double,
    seed: Int? = nil
) -> (DataFrame.Slice, DataFrame.Slice)
```

## Parameters 

`proportion`  

A proportion in the range `[0.0, 1.0]`.

`seed`  

A seed number for a random-number generator.

## Return Value

A tuple of two data frame slices.

## See Also

### Creating Two Slices by Splitting Rows

func randomSplit&lt;G>(by: Double, using: inout G) -> (DataFrame.Slice, DataFrame.Slice)

Generates two data frame slices by randomly splitting the rows of the data table type with a random-number generator.

