

- Accelerate
-  BNNSLayerParametersConvolution Deprecated

Structure

# BNNSLayerParametersConvolution

A structure that contains the parameters of a convolution layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
struct BNNSLayerParametersConvolution
```

Deprecated

Use BNNSGraph\* APIs

## Topics

### Initializers

init(i_desc: BNNSNDArrayDescriptor, w_desc: BNNSNDArrayDescriptor, o_desc: BNNSNDArrayDescriptor, bias: BNNSNDArrayDescriptor, activation: BNNSActivation, x_stride: Int, y_stride: Int, x_dilation_stride: Int, y_dilation_stride: Int, x_padding: Int, y_padding: Int, groups: Int, pad: (Int, Int, Int, Int))

Returns a new convolution layer parameters structure from the specified parameters.

init()

Returns a new convolution layer parameters structure.

### Instance Properties

var i_desc: BNNSNDArrayDescriptor

The descriptor of the input.

var w_desc: BNNSNDArrayDescriptor

The descriptor of the weights.

var o_desc: BNNSNDArrayDescriptor

The descriptor of the output.

var bias: BNNSNDArrayDescriptor

The bias descriptor.

var activation: BNNSActivation

The activation function that the layer applies to the output.

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

var groups: Int

Convolution group size.

var pad: (Int, Int, Int, Int)

Padding which is asymmetric and ignored if the width or height padding values are greater than zero.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Convolution layers

struct BNNSConvolutionLayerParameters

A structure containing convolution parameters.

Deprecated

func BNNSFilterCreateConvolutionLayer(UnsafePointer&lt;BNNSImageStackDescriptor>, UnsafePointer&lt;BNNSImageStackDescriptor>, UnsafePointer&lt;BNNSConvolutionLayerParameters>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a convolution filter, initialized with input, output, layer, and filter parameters.

Deprecated

class ConvolutionLayer

A layer object that wraps a convolution filter and manages its deinitialization.

Deprecated

func BNNSFilterCreateLayerConvolution(UnsafePointer&lt;BNNSLayerParametersConvolution>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new convolution layer.

Deprecated

func BNNSFilterCreateLayerTransposedConvolution(UnsafePointer&lt;BNNSLayerParametersConvolution>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new transposed convolution layer.

Deprecated

