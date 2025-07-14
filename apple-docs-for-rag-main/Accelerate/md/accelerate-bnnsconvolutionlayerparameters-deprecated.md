

- Accelerate
-  BNNSConvolutionLayerParameters Deprecated

Structure

# BNNSConvolutionLayerParameters

A structure containing convolution parameters.

iOS 10.0–14.0DeprecatediPadOS 10.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.12–11.0DeprecatedtvOS 10.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–7.0Deprecated

``` source
struct BNNSConvolutionLayerParameters
```

Deprecated

Use BNNSLayerParametersConvolution instead.

## Topics

### Initializers

init()

init(x_stride: Int, y_stride: Int, x_padding: Int, y_padding: Int, k_width: Int, k_height: Int, in_channels: Int, out_channels: Int, weights: BNNSLayerData, bias: BNNSLayerData, activation: BNNSActivation)

Returns a new convolution parameters structure.

init(x_stride: Int, y_stride: Int, x_padding: Int, y_padding: Int, k_width: Int, k_height: Int, in_channels: Int, out_channels: Int, weights: BNNSLayerData)

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

var weights: BNNSLayerData

Convolution weights.

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

### Convolution layers

func BNNSFilterCreateConvolutionLayer(UnsafePointer&lt;BNNSImageStackDescriptor>, UnsafePointer&lt;BNNSImageStackDescriptor>, UnsafePointer&lt;BNNSConvolutionLayerParameters>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a convolution filter, initialized with input, output, layer, and filter parameters.

Deprecated

class ConvolutionLayer

A layer object that wraps a convolution filter and manages its deinitialization.

Deprecated

struct BNNSLayerParametersConvolution

A structure that contains the parameters of a convolution layer.

Deprecated

func BNNSFilterCreateLayerConvolution(UnsafePointer&lt;BNNSLayerParametersConvolution>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new convolution layer.

Deprecated

func BNNSFilterCreateLayerTransposedConvolution(UnsafePointer&lt;BNNSLayerParametersConvolution>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new transposed convolution layer.

Deprecated

