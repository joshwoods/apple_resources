

- Accelerate
-  BNNSCropResize(\_:\_:\_:\_:\_:) Deprecated

Function

# BNNSCropResize(\_:\_:\_:\_:\_:)

Extracts and resizes regions of interest of an input tensor.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 9.0–11.0Deprecated

``` source
func BNNSCropResize(
    _ layer_params: UnsafePointer,
    _ input: UnsafePointer,
    _ roi: UnsafePointer,
    _ output: UnsafeMutablePointer,
    _ filter_params: UnsafePointer?
) -> Int32
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`layer_params`  

A pointer to the layer parameters.

`input`  

A pointer to the input array descriptor.

`roi`  

A pointer to the regions of interest array descriptor.

`output`  

A pointer to the output array descriptor.

`filter_params`  

Runtime filter parameters.

## Discussion

Use this function to resize the spatial dimensions (two dimensions with the smallest strides) of the first input according to the bounding boxes and box indices specified in the second input.

The operation works over contiguous 2D data and provides support for multiple channels and batches that contain more than one input-output pair.

For example, the following code defines a 6x5 matrix of single-precision values:

```
let batchSize = 1
let channelCount = 1

let values: [Float] = [ 0, 1, 0, 0, 0, 0,
                        1, 1, 1, 0, 0, 0,
                        0, 1, 0, 9, 0, 9,
                        0, 0, 0, 0, 9, 0,
                        0, 0, 0, 9, 0, 9 ]

var inputDescriptor = BNNSNDArrayDescriptor.allocate(
    initializingFrom: values,
    shape: .tensor4DLastMajor(6,
                              5,
                              channelCount,
                              batchSize))
```

Define the regions of interest as sets of four coordinates. The code below specifies the regions of interest with BNNSCenterSizeWidthFirst coordinate mode, that is the coordinates are ordered as horizontal center, vertical center, width, and height.

```
// Extracts:
//      0.0, 1.0, 0.0,
//      1.0, 1.0, 1.0,
//      0.0, 1.0, 0.0
let roiValues0: [Float] = [1, // w_center
                           1, // h_center
                           3, // box_width
                           3] // box_height

// Extracts:
//      9.0, 0.0, 9.0,
//      0.0, 9.0, 0.0,
//      9.0, 0.0, 9.0
let roiValues1: [Float] = [4, // w_center
                           3, // h_center
                           3, // box_width
                           3] // box_height
let boxCount = 2

var roiDescriptor = BNNSNDArrayDescriptor.allocate(
    initializingFrom: roiValues0 + roiValues1,
    shape: .matrixLastMajor(4,
                            boxCount))
```

Specify the output descriptor as a 5D tensor.

```
let outputWidth = 3
let outputHeight = 3

var outputDescriptor = BNNSNDArrayDescriptor.allocateUninitialized(
    scalarType: Float.self,
    shape: .tensor5DLastMajor(outputWidth,
                              outputHeight,
                              channelCount,
                              batchSize,
                              boxCount))
```

To perform the crop-resize, create a parameters structure and call BNNSCropResize(_:_:_:_:_:).

```
var params = BNNSLayerParametersCropResize(
    normalized_coordinates: false,
    spatial_scale: 1,
    extrapolation_value: 0,
    sampling_mode: BNNSLinearSamplingOffsetCorners,
    box_coordinate_mode: BNNSCenterSizeWidthFirst,
    method: BNNSInterpolationMethodLinear)

BNNSCropResize(&params,
               &inputDescriptor,
               &roiDescriptor,
               &outputDescriptor, nil)
```

On return, `outputDescriptor` contains `boxCount` slices that contain the data with the regions of interest of the input tensor:

```
[ 0.0, 1.0, 0.0,
  1.0, 1.0, 1.0,
  0.0, 1.0, 0.0,

  9.0, 0.0, 9.0,
  0.0, 9.0, 0.0,
  9.0, 0.0, 9.0 ]
```

## See Also

### Crop-resize layers

class CropResizeLayer

A layer object that wraps a crop-resize filter and manages its deinitialization.

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

