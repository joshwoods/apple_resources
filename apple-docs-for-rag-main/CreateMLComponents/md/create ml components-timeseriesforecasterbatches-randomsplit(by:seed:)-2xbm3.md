

- Create ML Components
- TimeSeriesForecasterBatches
-  randomSplit(by:seed:) 

Instance Method

# randomSplit(by:seed:)

Generates two AnnotatedFeatures by randomly splitting the elements of the sequence, at the same proportion within each unique Annotation.

Create ML ComponentsSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func randomSplit(
    by proportion: Double,
    seed: Int? = nil
) -> ([AnnotatedFeature], [AnnotatedFeature]) where Annotation : Hashable, Self.Element == AnnotatedFeature
```

## Parameters 

`proportion`  

A proportion in the range `[0.0, 1.0]`.

`seed`  

A seed number for a random-number generator.

## Return Value

A tuple of arrays.

