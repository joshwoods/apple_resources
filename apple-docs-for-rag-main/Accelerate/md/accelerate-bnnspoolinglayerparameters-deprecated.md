

- Accelerate
-  BNNSPoolingLayerParameters Deprecated

Structure

# BNNSPoolingLayerParameters

A structure containing pooling layer parameters.

iOS 10.0–14.0DeprecatediPadOS 10.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.12–11.0DeprecatedtvOS 10.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–7.0Deprecated

``` source
struct BNNSPoolingLayerParameters
```

Deprecated

Use BNNSLayerParametersPooling instead.

## Topics

### Initializers

init()

init(x_stride: Int, y_stride: Int, x_padding: Int, y_padding: Int, k_width: Int, k_height: Int, in_channels: Int, out_channels: Int, pooling_function: BNNSPoolingFunction, bias: BNNSLayerData, activation: BNNSActivation)

Returns a new pooling layer parameters structure

init(x_stride: Int, y_stride: Int, x_padding: Int, y_padding: Int, k_width: Int, k_height: Int, in_channels: Int, out_channels: Int, pooling_function: BNNSPoolingFunction)

### Instance Properties

var activation: BNNSActivation

The layer activation function.

var bias: BNNSLayerData

Layer bias, one for each output channel.

var in_channels: Int

The number of input channels.

var k_height: Int

The height of the convolution kernel.

var k_width: Int

The width of the convolution kernel.

var out_channels: Int

The number of output channels.

var pooling_function: BNNSPoolingFunction

The pooling function to apply to each sample.

var x_padding: Int

The X padding.

var x_stride: Int

The X increment in the input image.

var y_padding: Int

The Y padding.

var y_stride: Int

The Y increment in the input image.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Pooling layers

func BNNSFilterCreatePoolingLayer(UnsafePointer&lt;BNNSImageStackDescriptor>, UnsafePointer&lt;BNNSImageStackDescriptor>, UnsafePointer&lt;BNNSPoolingLayerParameters>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a pooling filter, initialized with input, output, layer, and filter parameters.

Deprecated

class PoolingLayer

A layer object that wraps a pooling filter and manages its deinitialization.

Deprecated

struct BNNSPoolingFunction

Constants that describe pooling functions.

var BNNSPoolingFunctionAverage: BNNSPoolingFunctionDeprecated

var BNNSPoolingFunctionMax: BNNSPoolingFunctionDeprecated

struct BNNSLayerParametersPooling

A structure that contains the parameters of a pooling layer.

Deprecated

func BNNSFilterCreateLayerPooling(UnsafePointer&lt;BNNSLayerParametersPooling>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new pooling layer.

Deprecated

func BNNSPoolingFilterApplyBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int, UnsafeMutablePointer&lt;Int>?, Int) -> Int32

Applies a pooling filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSPoolingFilterApplyBackwardBatch(BNNSFilter?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, UnsafePointer&lt;Int>?, Int) -> Int32

Applies a pooling filter backward to generate gradients.

Deprecated

func BNNSPoolingFilterApplyBatchEx(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutableRawPointer, Int, BNNSDataType, UnsafeMutableRawPointer?, Int) -> Int32

Applies a pooling filter to a set of input objects with support for multiple data types for indices.

Deprecated

func BNNSPoolingFilterApplyBackwardBatchEx(BNNSFilter?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int, UnsafeRawPointer?, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, BNNSDataType, UnsafeRawPointer?, Int) -> Int32

Applies a pooling filter backward to generate gradients with support for multiple data types for indices.

Deprecated

