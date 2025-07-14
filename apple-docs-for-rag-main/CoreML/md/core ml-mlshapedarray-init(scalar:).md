

- Core ML
- MLShapedArray
-  init(scalar:) 

Initializer

# init(scalar:)

Creates a shaped array with exactly one value and zero dimensions.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(scalar: Scalar)
```

## Parameters 

`scalar`  

A singular scalar value.

## Discussion

Use the shaped array’s `MLShapedArray/scalar` property to access the single value.

## See Also

### Creating a Shaped Array

init&lt;S>(scalars: S, shape: [Int])

Initialize with a sequence and the shape.

