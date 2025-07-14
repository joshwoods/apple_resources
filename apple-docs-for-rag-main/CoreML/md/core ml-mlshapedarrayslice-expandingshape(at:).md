

- Core ML
- MLShapedArraySlice
-  expandingShape(at:) 

Instance Method

# expandingShape(at:)

Returns a new shaped array with expanded dimensions

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
func expandingShape(at axis: Int) -> MLShapedArraySlice
```

Available when `Scalar` conforms to `MLShapedArrayScalar`.

## Discussion

The shape of the new `MLShapedArraySlice` gets a new dimension of 1 at the specified axis index.

```
let original = MLShapedArraySlice(scalars: 0..., shape: [2, 3])
let expanded = original.expanded(alongAxis: 0)
expanded.shape // [1, 2, 3]
```

