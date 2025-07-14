

- Accelerate
- BNNS
- BNNS.Shape
-  BNNS.Shape.tensor5DLastMajor(\_:\_:\_:\_:\_:stride:) 

Case

# BNNS.Shape.tensor5DLastMajor(\_:\_:\_:\_:\_:stride:)

A constant that represents a shape with a 5D last-major data layout.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
case tensor5DLastMajor(
    Int, Int, Int, Int, Int,
    stride: (Int, Int, Int, Int, Int) = (0, 0, 0, 0, 0)
)
```

## See Also

### Shape Constants

case vector(Int, stride: Int)

A constant that represents a shape with a 1D vector data layout.

case matrixColumnMajor(Int, Int, stride: (Int, Int))

A constant that represents a shape with a 2D column-major data layout.

case matrixRowMajor(Int, Int, stride: (Int, Int))

A constant that represents a shape with a 2D row-major data layout.

case matrixFirstMajor(Int, Int, stride: (Int, Int))

A constant that represents a shape with a 2D first-major data layout.

case matrixLastMajor(Int, Int, stride: (Int, Int))

A constant that represents a shape with a 2D last-major data layout.

case imageCHW(Int, Int, Int, stride: (Int, Int, Int))

A constant that represents a shape with a 3D image stack data layout.

case tensor3DFirstMajor(Int, Int, Int, stride: (Int, Int, Int))

A constant that represents a shape with a 3D first-major data layout.

case tensor3DLastMajor(Int, Int, Int, stride: (Int, Int, Int))

A constant that represents a shape with a 3D last-major data layout.

case tensor3DNSE(Int, Int, Int, stride: (Int, Int, Int))

A constant that represents a shape with the size elements embedding dimension, sequence length, and batch size.

case tensor3DSNE(Int, Int, Int, stride: (Int, Int, Int))

A constant that represents a shape with the size elements embedding dimension, batch size, and sequence length.

case convolutionWeightsOIHW(Int, Int, Int, Int, stride: (Int, Int, Int, Int))

A constant that represents a shape with a 4D array of convolution weights data layout.

case tensor4DFirstMajor(Int, Int, Int, Int, stride: (Int, Int, Int, Int))

A constant that represents a shape with a 4D first-major data layout.

case tensor4DLastMajor(Int, Int, Int, Int, stride: (Int, Int, Int, Int))

A constant that represents a shape with a 4D last-major data layout.

case tensor5DFirstMajor(Int, Int, Int, Int, Int, stride: (Int, Int, Int, Int, Int))

A constant that represents a shape with a 5D first-major data layout.

case tensor6DFirstMajor(Int, Int, Int, Int, Int, Int, stride: (Int, Int, Int, Int, Int, Int))

A constant that represents a shape with a 6D first-major data layout.

