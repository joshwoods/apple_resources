

- Core ML
- MLShapedArraySlice
-  transposed() 

Instance Method

# transposed()

Returns a new transposed shaped array

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
func transposed() -> MLShapedArraySlice
```

Available when `Scalar` conforms to `MLShapedArrayScalar`.

## Discussion

This is equivalent to `transposed(permutation:)` where `permutation:` parameter is `[shape.count-1, shape.count-2, ..., 0]`, which reverses the shape.

```
let original = MLShapedArraySlice(scalars: 0..., shape: [1, 2, 3])
let transposed = original.transposed()
transposed.shape // [3, 2, 1]
```

