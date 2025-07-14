

- Create ML
- MLDataTable
- MLDataTable.Row
- MLDataTable.Row.Values
-  randomSplit(by:seed:) 

Instance Method

# randomSplit(by:seed:)

Generates two generic arrays by randomly splitting the elements of the sequence.

Create MLSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func randomSplit(
    by proportion: Double,
    seed: Int? = nil
) -> (ArraySlice, ArraySlice) where T == Self.Element
```

## Parameters 

`proportion`  

A proportion in the range `[0.0, 1.0]`.

`seed`  

A seed number for a random-number generator.

## Return Value

A tuple of array slices.

