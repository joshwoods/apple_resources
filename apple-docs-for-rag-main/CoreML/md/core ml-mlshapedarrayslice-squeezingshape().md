

- Core ML
- MLShapedArraySlice
-  squeezingShape() 

Instance Method

# squeezingShape()

Returns a new squeezed shaped array.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
func squeezingShape() -> MLShapedArraySlice
```

Available when `Scalar` conforms to `MLShapedArrayScalar`.

## Discussion

The new shape removes 1s in the original shape.

```
let original = MLShapedArraySlice(scalars: 0..., shape: [1, 2, 1, 2])
let squeezed = original.squeezed()
squeezed.shape // [2, 2]
```

When all the dimensions of the original shape is one, the resultant shaped array is a scalar.

```
let original = MLShapedArray(scalars: 42, shape: [1, 1])
let squeezed = original.squeezed()
squeezed.scalar // 42
```

