

- ML Compute
-  MLCConvolutionType Deprecated

Enumeration

# MLCConvolutionType

The convolution type specified for a convolution layer.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
enum MLCConvolutionType
```

## Topics

### Enumeration Cases

case standard

case depthwise

case transposed

var debugDescription: String

A textual description of the convolution type, suitable for debugging.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating Convolution Descriptors

convenience init(type: MLCConvolutionType, kernelSizes: (height: Int, width: Int), inputFeatureChannelCount: Int, outputFeatureChannelCount: Int, groupCount: Int, strides: (y: Int, x: Int), dilationRates: (y: Int, x: Int), paddingPolicy: MLCPaddingPolicy)

Creates a descriptor for the type, sizes, number of feature channels, group count, strides, dilation rates, and padding policy you specify.

Deprecated

convenience init(transposeWithKernelWidth: Int, kernelHeight: Int, inputFeatureChannelCount: Int, outputFeatureChannelCount: Int)

Creates a descriptor for convolution transpose with the kernel sizes and number of feature channels you specify.

Deprecated

convenience init(depthwiseWithKernelWidth: Int, kernelHeight: Int, inputFeatureChannelCount: Int, channelMultiplier: Int)

Creates a descriptor for depthwise convolution with the kernel sizes, number of input feature channels, and channel multiplier you specify.

Deprecated

