

- Accelerate
- BNNS
-  BNNS.DataLayout 

Enumeration

# BNNS.DataLayout

Constants that describe the data layout of an n-dimensional array descriptor shape.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
enum DataLayout
```

## Topics

### Data Layout Constants

case vector

A constant that represents a 1D vector.

case matrixColumnMajor

A constant that represents a 2D column-major matrix.

case matrixRowMajor

A constant that represents a 2D row-major matrix.

case matrixFirstMajor

A constant that represents a 2D first-major matrix.

case matrixLastMajor

A constant that represents a 2D last-major matrix.

case imageCHW

A constant that represents a 3D image stack.

case tensor3DFirstMajor

A constant that represents a 3D first-major tensor.

case tensor3DLastMajor

A constant that represents a 3D last-major tensor.

case tensor3DNSE

A constant that represents a 3D tensor with size ordered by embedding dimension, sequence length, batch size.

case tensor3DSNE

A constant that represents a 3D tensor with size ordered by embedding dimension, batch size, sequence length.

case convolutionWeightsOIHW

A constant that represents a 4D array of convolution weights.

case tensor4DFirstMajor

A constant that represents a 4D first-major tensor.

case tensor4DLastMajor

A constant that represents a 4D last-major tensor.

case tensor5DFirstMajor

A constant that represents a 5D first-major tensor.

case tensor5DLastMajor

A constant that represents a 5D last-major tensor.

case tensor6DFirstMajor

A constant that represents a 6D first-major tensor.

case tensor6DLastMajor

A constant that represents a 6D last-major tensor.

case tensor7DFirstMajor

A constant that represents a 7D first-major tensor.

case tensor7DLastMajor

A constant that represents a 7D last-major tensor.

case tensor8DFirstMajor

A constant that represents a 8D first-major tensor.

case tensor8DLastMajor

A constant that represents a 8D last-major tensor.

### Determining the Number of Dimensions

var rank: Int

The number of dimensions of the data layout.

## Relationships

### Conforms To

- CaseIterable
- Copyable
- Equatable
- Hashable

