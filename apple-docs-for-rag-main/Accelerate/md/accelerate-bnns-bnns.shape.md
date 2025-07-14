

- Accelerate
- BNNS
-  BNNS.Shape 

Enumeration

# BNNS.Shape

Constants that describe the size and data layout of an n-dimensional array descriptor.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
enum Shape
```

## Topics

### Creating a Shape

init([Int], dataLayout: BNNS.DataLayout?, stride: [Int]?)

Returns a new shape with the specified size, data layout, and stride.

init(arrayLiteral: BNNS.Shape.ArrayLiteralElement...)

Returns a new shape with the specified size.

### Specifying the Data Layout of a Shape

enum DataLayout

Constants that describe the data layout of an n-dimensional array descriptor shape.

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

case tensor5DLastMajor(Int, Int, Int, Int, Int, stride: (Int, Int, Int, Int, Int))

A constant that represents a shape with a 5D last-major data layout.

case tensor6DFirstMajor(Int, Int, Int, Int, Int, Int, stride: (Int, Int, Int, Int, Int, Int))

A constant that represents a shape with a 6D first-major data layout.

case tensor6DLastMajor(Int, Int, Int, Int, Int, Int, stride: (Int, Int, Int, Int, Int, Int))

A constant that represents a shape with a 6D last-major data layout.

case tensor7DFirstMajor(Int, Int, Int, Int, Int, Int, Int, stride: (Int, Int, Int, Int, Int, Int, Int))

A constant that represents a shape with a 7D first-major data layout.

case tensor7DLastMajor(Int, Int, Int, Int, Int, Int, Int, stride: (Int, Int, Int, Int, Int, Int, Int))

A constant that represents a shape with a 7D last-major data layout.

case tensor8DFirstMajor(Int, Int, Int, Int, Int, Int, Int, Int, stride: (Int, Int, Int, Int, Int, Int, Int, Int))

A constant that represents a shape with a 8D first-major data layout.

case tensor8DLastMajor(Int, Int, Int, Int, Int, Int, Int, Int, stride: (Int, Int, Int, Int, Int, Int, Int, Int))

A constant that represents a shape with a 8D last-major data layout.

### Inspecting the Properties of a Shape

var batchStride: Int

The number of elements between each batch of data in the shape.

var layout: BNNSDataLayout

The data layout of the shape.

var rank: Int

The number of dimensions of the shape.

var size: (Int, Int, Int, Int, Int, Int, Int, Int)

The size, in elements, of each dimension of the shape.

var stride: (Int, Int, Int, Int, Int, Int, Int, Int)

The stride, in elements, of each dimension of the shape.

### Default Implementations

ExpressibleByArrayLiteral Implementations

## Relationships

### Conforms To

- Copyable
- ExpressibleByArrayLiteral

## See Also

### N-dimensional array descriptor essentials

struct BNNSLayerData

A structure containing common layer parameters.

Deprecated

struct BNNSDataLayout

Constants that describe the data type of an n-dimensional array.

struct BNNSDataType

BNNS Data Types.

struct BNNSNDArrayDescriptor

A structure that describes the shape, stride, data type, and, optionally, the memory location of an n-dimensional array.

func BNNSDataLayoutGetRank(BNNSDataLayout) -> Int

