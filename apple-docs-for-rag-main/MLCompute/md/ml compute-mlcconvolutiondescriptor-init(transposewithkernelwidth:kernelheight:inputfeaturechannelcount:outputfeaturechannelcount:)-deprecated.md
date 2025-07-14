

- ML Compute
- MLCConvolutionDescriptor
-  init(transposeWithKernelWidth:kernelHeight:inputFeatureChannelCount:outputFeatureChannelCount:) Deprecated

Initializer

# init(transposeWithKernelWidth:kernelHeight:inputFeatureChannelCount:outputFeatureChannelCount:)

Creates a descriptor for convolution transpose with the kernel sizes and number of feature channels you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init(
    transposeWithKernelWidth kernelWidth: Int,
    kernelHeight: Int,
    inputFeatureChannelCount: Int,
    outputFeatureChannelCount: Int
)
```

## Parameters 

`kernelWidth`  

The kernel size in x.

`kernelHeight`  

The kernel size in y.

`inputFeatureChannelCount`  

The number of feature channels in the input tensor.

`outputFeatureChannelCount`  

The number of feature channels in the output tensor.

## See Also

### Creating Convolution Descriptors

convenience init(type: MLCConvolutionType, kernelSizes: (height: Int, width: Int), inputFeatureChannelCount: Int, outputFeatureChannelCount: Int, groupCount: Int, strides: (y: Int, x: Int), dilationRates: (y: Int, x: Int), paddingPolicy: MLCPaddingPolicy)

Creates a descriptor for the type, sizes, number of feature channels, group count, strides, dilation rates, and padding policy you specify.

Deprecated

convenience init(depthwiseWithKernelWidth: Int, kernelHeight: Int, inputFeatureChannelCount: Int, channelMultiplier: Int)

Creates a descriptor for depthwise convolution with the kernel sizes, number of input feature channels, and channel multiplier you specify.

Deprecated

enum MLCConvolutionType

The convolution type specified for a convolution layer.

Deprecated

