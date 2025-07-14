

- ML Compute
-  MLCConvolutionDescriptor Deprecated

Class

# MLCConvolutionDescriptor

A configuration object you use to create a convolution or fully connected layer.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCConvolutionDescriptor
```

## Topics

### Creating Convolution Descriptors

convenience init(type: MLCConvolutionType, kernelSizes: (height: Int, width: Int), inputFeatureChannelCount: Int, outputFeatureChannelCount: Int, groupCount: Int, strides: (y: Int, x: Int), dilationRates: (y: Int, x: Int), paddingPolicy: MLCPaddingPolicy)

Creates a descriptor for the type, sizes, number of feature channels, group count, strides, dilation rates, and padding policy you specify.

convenience init(transposeWithKernelWidth: Int, kernelHeight: Int, inputFeatureChannelCount: Int, outputFeatureChannelCount: Int)

Creates a descriptor for convolution transpose with the kernel sizes and number of feature channels you specify.

convenience init(depthwiseWithKernelWidth: Int, kernelHeight: Int, inputFeatureChannelCount: Int, channelMultiplier: Int)

Creates a descriptor for depthwise convolution with the kernel sizes, number of input feature channels, and channel multiplier you specify.

enum MLCConvolutionType

The convolution type specified for a convolution layer.

### Inspecting Convolution Descriptors

var convolutionType: MLCConvolutionType

The type of convolution.

var kernelSizes: (height: Int, width: Int)

A tuple that contains the kernel sizes for height and width.

var inputFeatureChannelCount: Int

The number of feature channels in the input tensor.

var outputFeatureChannelCount: Int

The number of feature channels in the output tensor.

var strides: (y: Int, x: Int)

A tuple that contains the kernel strides for y and x.

var dilationRates: (y: Int, x: Int)

A tuple that contains the dilation rates for y and x.

var groupCount: Int

The number of groups.

var paddingPolicy: MLCPaddingPolicy

The padding policy.

var isConvolutionTranspose: Bool

A Boolean that indicates whether this is a convolution transpose.

var usesDepthwiseConvolution: Bool

A Boolean that indicates whether you use depthwise convolution.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Creating Convolution Layers

convenience init?(weights: MLCTensor, biases: MLCTensor?, descriptor: MLCConvolutionDescriptor)

Creates a convolution layer with the weights, biases, and descriptor you specify.

Deprecated

