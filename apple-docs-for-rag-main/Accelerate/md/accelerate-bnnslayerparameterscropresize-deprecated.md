

- Accelerate
-  BNNSLayerParametersCropResize Deprecated

Structure

# BNNSLayerParametersCropResize

A set of parameters that describe a crop-resize operation.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
struct BNNSLayerParametersCropResize
```

Deprecated

Use BNNSGraph\* APIs

## Topics

### Initializers

init(normalized_coordinates: Bool, spatial_scale: Float, extrapolation_value: Float, sampling_mode: BNNSLinearSamplingMode, box_coordinate_mode: BNNSBoxCoordinateMode, method: BNNSInterpolationMethod)

Creates a new layer parameters structure.

init()

Creates a new empty layer parameters structure.

### Instance Properties

var normalized_coordinates: Bool

A Boolean value that specifies whether the operation treats the coordinates as normalized to `0...1`.

var spatial_scale: Float

An additional spatial scale that mutliplies the bounding box coordinates.

var extrapolation_value: Float

A value that the operation uses for extrapolation. Default value is `0`.

var sampling_mode: BNNSLinearSamplingMode

The sampling mode that the operation uses to select sample points.

var box_coordinate_mode: BNNSBoxCoordinateMode

A constant that defines the convention that the operation uses to specify the four bounding box coordinates.

var method: BNNSInterpolationMethod

The interpolation method.

## Relationships

### Conforms To

- BitwiseCopyable
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

struct BNNSBoxCoordinateMode

Constants that define the convention to specify the four bounding box coordinates for crop-resize operations.

struct BNNSLinearSamplingMode

Constants that specify how a crop-resize layer samples a grid.

