

- Accelerate
-  BNNSLinearSamplingMode 

Structure

# BNNSLinearSamplingMode

Constants that specify how a crop-resize layer samples a grid.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSLinearSamplingMode
```

## Topics

### Constants

init(UInt32)

init(rawValue: UInt32)

var rawValue: UInt32

var BNNSLinearSamplingDefault: BNNSLinearSamplingMode

The default linear sampling mode.

var BNNSLinearSamplingAlignCorners: BNNSLinearSamplingMode

The align corners sampling mode.

var BNNSLinearSamplingUnalignCorners: BNNSLinearSamplingMode

The unalign corners sampling mode.

var BNNSLinearSamplingStrictAlignCorners: BNNSLinearSamplingMode

The strict align corners sampling mode.

var BNNSLinearSamplingOffsetCorners: BNNSLinearSamplingMode

The offset corners sampling mode.

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

struct BNNSBoxCoordinateMode

Constants that define the convention to specify the four bounding box coordinates for crop-resize operations.

