

- Accelerate
-  BNNSLayerParametersPooling Deprecated

Structure

# BNNSLayerParametersPooling

A structure that contains the parameters of a pooling layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
struct BNNSLayerParametersPooling
```

Deprecated

Use BNNSGraph\* APIs

## Topics

### Initializers

init(i_desc: BNNSNDArrayDescriptor, o_desc: BNNSNDArrayDescriptor, bias: BNNSNDArrayDescriptor, activation: BNNSActivation, pooling_function: BNNSPoolingFunction, k_width: Int, k_height: Int, x_stride: Int, y_stride: Int, x_dilation_stride: Int, y_dilation_stride: Int, x_padding: Int, y_padding: Int, pad: (Int, Int, Int, Int))

Returns a new pooling layer parameters structure from the specified parameters.

init()

Returns a new pooling layer parameters structure.

### Instance Properties

var i_desc: BNNSNDArrayDescriptor

The descriptor of the input.

var o_desc: BNNSNDArrayDescriptor

The descriptor of the output.

var bias: BNNSNDArrayDescriptor

The descriptor of the bias.

var activation: BNNSActivation

The activation function that the layer applies to the output.

var pooling_function: BNNSPoolingFunction

The variable that specifies the pooling function.

var k_width: Int

The width of the kernel.

var k_height: Int

The height of the kernel.

var x_stride: Int

The width increment of the input image.

var y_stride: Int

The height increment of the input image.

var x_dilation_stride: Int

The width increment between elements in the input image during convolution.

var y_dilation_stride: Int

The height increment between elements in the input image during convolution.

var x_padding: Int

The width padding, which is the number of virtual zeros added to the left and right of each channel.

var y_padding: Int

The height padding, which is the number of virtual zeros added to the top and bottom of each channel.

var pad: (Int, Int, Int, Int)

Asymmetric padding, ignored if `x_padding` or `y_padding` are greater than zero.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Pooling layers

struct BNNSPoolingLayerParameters

A structure containing pooling layer parameters.

Deprecated

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

