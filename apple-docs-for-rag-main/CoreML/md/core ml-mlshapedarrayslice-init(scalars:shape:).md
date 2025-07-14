

- Core ML
- MLShapedArraySlice
-  init(scalars:shape:) 

Initializer

# init(scalars:shape:)

Initialize with a sequence and the shape.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
init(
    scalars: S,
    shape: [Int]
) where Scalar == S.Element, S : Sequence
```

## Parameters 

`scalars`  

The initializing sequence.

`shape`  

The shape

## Discussion

The length of the sequence must not be less than the number of scalars in the shaped array.

## See Also

### Creating a Shaped Array Slice

init(scalar: Scalar)

Creates a shaped array slice with exactly one value and zero dimensions.

