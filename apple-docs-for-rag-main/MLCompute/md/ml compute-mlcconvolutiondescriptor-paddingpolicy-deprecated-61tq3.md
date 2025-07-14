

- ML Compute
- MLCConvolutionDescriptor
-  paddingPolicy Deprecated

Instance Property

# paddingPolicy

The padding policy.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
var paddingPolicy: MLCPaddingPolicy { get }
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## See Also

### Inspecting Convolution Descriptors

var convolutionType: MLCConvolutionType

The type of convolution.

Deprecated

var kernelSizes: (height: Int, width: Int)

A tuple that contains the kernel sizes for height and width.

Deprecated

var inputFeatureChannelCount: Int

The number of feature channels in the input tensor.

Deprecated

var outputFeatureChannelCount: Int

The number of feature channels in the output tensor.

Deprecated

var strides: (y: Int, x: Int)

A tuple that contains the kernel strides for y and x.

Deprecated

var dilationRates: (y: Int, x: Int)

A tuple that contains the dilation rates for y and x.

Deprecated

var groupCount: Int

The number of groups.

Deprecated

var isConvolutionTranspose: Bool

A Boolean that indicates whether this is a convolution transpose.

Deprecated

var usesDepthwiseConvolution: Bool

A Boolean that indicates whether you use depthwise convolution.

Deprecated

