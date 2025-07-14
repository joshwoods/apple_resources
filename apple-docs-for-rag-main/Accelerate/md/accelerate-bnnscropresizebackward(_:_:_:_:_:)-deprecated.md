

- Accelerate
-  BNNSCropResizeBackward(\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSCropResizeBackward(\_:\_:\_:\_:\_:)

Applies a crop-resize filter backward to generate gradients.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
func BNNSCropResizeBackward(
    _ layer_params: UnsafePointer,
    _ in_delta: UnsafeMutablePointer,
    _ roi: UnsafePointer,
    _ out_delta: UnsafePointer,
    _ filter_params: UnsafePointer?
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`layer_params`  

A pointer to the layer parameters.

`in_delta`  

A pointer to the input delta descriptor.

`roi`  

A pointer to the regions of interest array descriptor.

`out_delta`  

A pointer to the output delta descriptor.

`filter_params`  

Runtime filter parameters.

## See Also

### Crop-resize layers

class CropResizeLayer

A layer object that wraps a crop-resize filter and manages its deinitialization.

Deprecated

func BNNSCropResize(UnsafePointer&lt;BNNSLayerParametersCropResize>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSNDArrayDescriptor>, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Extracts and resizes regions of interest of an input tensor.

Deprecated

struct BNNSLayerParametersCropResize

A set of parameters that describe a crop-resize operation.

Deprecated

struct BNNSBoxCoordinateMode

Constants that define the convention to specify the four bounding box coordinates for crop-resize operations.

struct BNNSLinearSamplingMode

Constants that specify how a crop-resize layer samples a grid.

