

- Core ML
- MLShapedArraySlice
-  transposed(permutation:) 

Instance Method

# transposed(permutation:)

Returns a new transposed shaped array using a custom permutation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
func transposed(permutation axes: [Int]) -> MLShapedArraySlice
```

Available when `Scalar` conforms to `MLShapedArrayScalar`.

## Discussion

Use this method to convert, for example, the image data layout from `[C, H, W]` to `[C, W, H]`, where `C` is channel, `W` is width, and `H` is height.

```
// The source tensor has 3 channels, 128 x 64 image in [C, H, W] layout.
let imageCHW = MLShapedArray(scalars: pixelValues,
                                    shape: [3, 64, 128])
// Slice for the first two channels.
let imageSliceCHW = imageCHW[0..

The shape (`shape_out`) is transposed from the input shape (`shape_in`) as follows.

```
shape_out[i]
  == permutation.map { shape_in[$0] }
```

The scalar value of the output shaped array (`array_out`) is related to the input shaped array (`array_in`) as follows.

```
array_out(scalarAt: permutation.map { indices[$0] })
  == array_in[scalarAt: indices]]
```

