

- Accelerate
- BNNSLayerParametersConvolution
-  bias Deprecated

Instance Property

# bias

The bias descriptor.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
var bias: BNNSNDArrayDescriptor
```

Deprecated

Use BNNSGraph\* APIs

## See Also

### Instance Properties

var i_desc: BNNSNDArrayDescriptor

The descriptor of the input.

Deprecated

var w_desc: BNNSNDArrayDescriptor

The descriptor of the weights.

Deprecated

var o_desc: BNNSNDArrayDescriptor

The descriptor of the output.

Deprecated

var activation: BNNSActivation

The activation function that the layer applies to the output.

Deprecated

var x_stride: Int

The width increment of the input image.

Deprecated

var y_stride: Int

The height increment of the input image.

Deprecated

var x_dilation_stride: Int

The width increment between elements in the input image during convolution.

Deprecated

var y_dilation_stride: Int

The height increment between elements in the input image during convolution.

Deprecated

var x_padding: Int

The width padding, which is the number of virtual zeros added to the left and right of each channel.

Deprecated

var y_padding: Int

The height padding, which is the number of virtual zeros added to the top and bottom of each channel.

Deprecated

var groups: Int

Convolution group size.

Deprecated

var pad: (Int, Int, Int, Int)

Padding which is asymmetric and ignored if the width or height padding values are greater than zero.

Deprecated

