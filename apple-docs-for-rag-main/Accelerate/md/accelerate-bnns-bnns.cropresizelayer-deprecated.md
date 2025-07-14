

- Accelerate
- BNNS
-  BNNS.CropResizeLayer Deprecated

Class

# BNNS.CropResizeLayer

A layer object that wraps a crop-resize filter and manages its deinitialization.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
class CropResizeLayer
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Creating a Crop-Resize Layer

init(coordinatesAreNormalized: Bool, spatialScale: Float, extrapolationValue: Float, samplingMode: BNNS.CropResizeLayer.LinearSamplingMode, boxCoordinateMode: BNNS.CropResizeLayer.BoxCoordinateMode)

Returns a new crop-resize layer.

### Applying a Crop-Resize Layer

func apply(input: BNNSNDArrayDescriptor, regionOfInterest: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, filterParameters: BNNSFilterParameters?) throws

Applies the layer to a set of input objects, writing the result to a set of output objects.

func applyBackward(regionOfInterest: BNNSNDArrayDescriptor, outputGradient: BNNSNDArrayDescriptor, generatingInputGradient: BNNSNDArrayDescriptor, filterParameters: BNNSFilterParameters?) throws

Applies a crop-resize filter backward to generate an input gradient.

### Suporting Types

enum BoxCoordinateMode

An enumeration that defines the convention for specifying the bounding box coordinates of a 2D image.

enum LinearSamplingMode

An enumeration that specifies the interpolation sampling mode.

## See Also

### Crop-resize layers

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

struct BNNSLinearSamplingMode

Constants that specify how a crop-resize layer samples a grid.

