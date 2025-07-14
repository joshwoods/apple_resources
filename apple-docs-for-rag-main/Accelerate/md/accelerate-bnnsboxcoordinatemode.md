

- Accelerate
-  BNNSBoxCoordinateMode 

Structure

# BNNSBoxCoordinateMode

Constants that define the convention to specify the four bounding box coordinates for crop-resize operations.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSBoxCoordinateMode
```

## Topics

### Constants

init(UInt32)

init(rawValue: UInt32)

var rawValue: UInt32

var BNNSCenterSizeHeightFirst: BNNSBoxCoordinateMode

Specifies coordinates as corners with the order: height start, width start, height end, width end.

var BNNSCenterSizeWidthFirst: BNNSBoxCoordinateMode

Specifies coordinates as corners with the order: width start, height start, width end, height end.

var BNNSCornersHeightFirst: BNNSBoxCoordinateMode

Specifies coordinates as center and size with the order: height center, width center, height, width.

var BNNSCornersWidthFirst: BNNSBoxCoordinateMode

Specifies coordinates as center and size with the order: width center, height center, width, height.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Crop-resize layers

class CropResizeLayer

A layer object that wraps a crop-resize filter and manages its deinitialization.

Deprecated

func BNNSCropResize(UnsafePointer&lt;BNNSLayerParametersCropResize>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Extracts and resizes regions of interest of an input tensor.

Deprecated

func BNNSCropResizeBackward(UnsafePointer&lt;BNNSLayerParametersCropResize>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Applies a crop-resize filter backward to generate gradients.

Deprecated

struct BNNSLayerParametersCropResize

A set of parameters that describe a crop-resize operation.

Deprecated

struct BNNSLinearSamplingMode

Constants that specify how a crop-resize layer samples a grid.

