

- Create ML
- MLDataTable
- MLDataTable.Rows
-  randomSplit(by:using:) 

Instance Method

# randomSplit(by:using:)

Generates two AnnotatedFeatures by randomly splitting the elements of the sequence, at the same proportion within each unique Annotation.

Create MLSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func randomSplit(
    by proportion: Double,
    using generator: inout Generator
) -> ([AnnotatedFeature], [AnnotatedFeature]) where Annotation : Hashable, Generator : RandomNumberGenerator, Self.Element == AnnotatedFeature
```

## Parameters 

`proportion`  

A proportion in the range `[0.0, 1.0]`.

`generator`  

A random-number generator.

## Return Value

A tuple of arrays.

