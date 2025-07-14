

- Core ML
- MLShapedArraySlice
-  reshaped(to:) 

Instance Method

# reshaped(to:)

Returns a new reshaped shaped array.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
func reshaped(to newShape: [Int]) -> MLShapedArraySlice
```

Available when `Scalar` conforms to `MLShapedArrayScalar`.

## Parameters 

`newShape`  

The new shape after reshaping.

## Discussion

The reshaped array gets scalars of the original array in first-major order. Therefore, the initializer is semantically equivalent to:

```
let reshaped = MLShapedArray(scalars: original.scalars, shape: newShape)
```

Usage example:

```
let original = MLShapedArraySlice(scalars: 0..., shape: [4])
let reshaped = original.reshaped(to: [1, 2, 2])
```

A scalar can be reshaped to and from a shape where the product of dimensions is one.

The method raises a runtime error if the product of dimensions in the new shape is different from the current one.

