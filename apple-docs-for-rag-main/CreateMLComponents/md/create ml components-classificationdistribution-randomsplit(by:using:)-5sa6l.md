

- Create ML Components
- ClassificationDistribution
-  randomSplit(by:using:) 

Instance Method

# randomSplit(by:using:)

Generates two generic arrays by randomly splitting the elements of the sequence.

Create ML ComponentsSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func randomSplit(
    by proportion: Double,
    using generator: inout Generator
) -> (ArraySlice, ArraySlice) where T == Self.Element, Generator : RandomNumberGenerator
```

## Parameters 

`proportion`  

A proportion in the range `[0.0, 1.0]`.

`generator`  

A random-number generator.

## Return Value

A tuple of array slices.

