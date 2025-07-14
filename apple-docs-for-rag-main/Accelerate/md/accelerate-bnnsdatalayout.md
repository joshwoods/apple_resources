

- Accelerate
-  BNNSDataLayout 

Structure

# BNNSDataLayout

Constants that describe the data type of an n-dimensional array.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSDataLayout
```

## Topics

### 1D Data Layouts

var BNNSDataLayoutVector: BNNSDataLayout

A constant that represents a 1D vector.

var BNNSDataLayout1DFirstMajor: BNNSDataLayout

A constant that represents a 1D first-major vector.

var BNNSDataLayout1DLastMajor: BNNSDataLayout

A constant that represents a 1D last-major vector.

### 2D Data Layouts

var BNNSDataLayoutColumnMajorMatrix: BNNSDataLayout

A constant that represents a 2D column-major matrix.

var BNNSDataLayoutRowMajorMatrix: BNNSDataLayout

A constant that represents a 2D row-major matrix.

var BNNSDataLayout2DFirstMajor: BNNSDataLayout

A constant that represents a 2D first-major matrix.

var BNNSDataLayout2DLastMajor: BNNSDataLayout

A constant that represents a 2D last-major matrix.

### 3D Data Layouts

var BNNSDataLayoutImageCHW: BNNSDataLayout

A constant that represents a 3D image stack.

var BNNSDataLayout3DFirstMajor: BNNSDataLayout

A constant that represents a 3D first-major tensor.

var BNNSDataLayout3DLastMajor: BNNSDataLayout

A constant that represents a 3D last-major tensor.

var BNNSDataLayoutSNE: BNNSDataLayout

A constant that represents a 3D tensor with the size elements embedding dimension, batch size, and sequence length.

var BNNSDataLayoutNSE: BNNSDataLayout

A constant that represents a 3D tensor with the size elements embedding dimension, sequence length, and batch size.

### 4D Data Layouts

var BNNSDataLayoutConvolutionWeightsOIHW: BNNSDataLayout

A constant that represents a 4D array of convolution weights.

var BNNSDataLayoutConvolutionWeightsIOHrWr: BNNSDataLayout

A constant that represents a 4D array of rotated convolution weights.

var BNNSDataLayoutConvolutionWeightsOIHrWr: BNNSDataLayout

A constant that represents a 4D array of rotated convolution weights.

var BNNSDataLayoutConvolutionWeightsOIHW_Pack32: BNNSDataLayout

A constant that represents a 4D array of packed convolution weights with 32-output channel packing and 128-byte array address alignment.

var BNNSDataLayout4DFirstMajor: BNNSDataLayout

A constant that represents a 4D first-major tensor.

var BNNSDataLayout4DLastMajor: BNNSDataLayout

A constant that represents a 4D last-major tensor.

### 5D Data Layouts

var BNNSDataLayout5DFirstMajor: BNNSDataLayout

A constant that represents a 5D first-major tensor.

var BNNSDataLayout5DLastMajor: BNNSDataLayout

A constant that represents a 5D last-major tensor.

### 6D Data Layouts

var BNNSDataLayout6DFirstMajor: BNNSDataLayout

A constant that represents a 6D first-major tensor.

var BNNSDataLayout6DLastMajor: BNNSDataLayout

A constant that represents a 6D last-major tensor.

### 7D Data Layouts

var BNNSDataLayout7DFirstMajor: BNNSDataLayout

A constant that represents a 7D first-major tensor.

var BNNSDataLayout7DLastMajor: BNNSDataLayout

A constant that represents a 7D last-major tensor.

### 8D Data Layouts

var BNNSDataLayout8DFirstMajor: BNNSDataLayout

A constant that represents a 8D first-major tensor.

var BNNSDataLayout8DLastMajor: BNNSDataLayout

A constant that represents a 8D last-major tensor.

### Other Data Layouts

var BNNSDataLayoutFullyConnectedSparse: BNNSDataLayout

var BNNSDataLayoutMHA_DHK: BNNSDataLayout

### Raw Values

init(UInt32)

init(rawValue: UInt32)

var rawValue: UInt32

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### N-dimensional array descriptor essentials

struct BNNSLayerData

A structure containing common layer parameters.

Deprecated

enum Shape

Constants that describe the size and data layout of an n-dimensional array descriptor.

struct BNNSDataType

BNNS Data Types.

struct BNNSNDArrayDescriptor

A structure that describes the shape, stride, data type, and, optionally, the memory location of an n-dimensional array.

func BNNSDataLayoutGetRank(BNNSDataLayout) -> Int

