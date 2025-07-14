

- ML Compute
- MLCConvolutionDescriptor
-  convolutionType Deprecated

Instance Property

# convolutionType

The type of convolution.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var convolutionType: MLCConvolutionType { get }
```

## See Also

### Inspecting Convolution Descriptors

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

var paddingPolicy: MLCPaddingPolicy

The padding policy.

Deprecated

var isConvolutionTranspose: Bool

A Boolean that indicates whether this is a convolution transpose.

Deprecated

var usesDepthwiseConvolution: Bool

A Boolean that indicates whether you use depthwise convolution.

Deprecated

