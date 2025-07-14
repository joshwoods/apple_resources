

- ML Compute
- MLCConvolutionDescriptor
-  init(type:kernelSizes:inputFeatureChannelCount:outputFeatureChannelCount:groupCount:strides:dilationRates:paddingPolicy:) Deprecated

Initializer

# init(type:kernelSizes:inputFeatureChannelCount:outputFeatureChannelCount:groupCount:strides:dilationRates:paddingPolicy:)

Creates a descriptor for the type, sizes, number of feature channels, group count, strides, dilation rates, and padding policy you specify.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
convenience init(
    type: MLCConvolutionType = .standard,
    kernelSizes: (height: Int, width: Int),
    inputFeatureChannelCount: Int,
    outputFeatureChannelCount: Int,
    groupCount: Int = 1,
    strides: (y: Int, x: Int) = (1, 1),
    dilationRates: (y: Int, x: Int) = (1, 1),
    paddingPolicy: MLCPaddingPolicy = .same
)
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## Parameters 

`type`  

The convolution type.

`kernelSizes`  

A tuple that contains the kernel sizes for y and x.

`inputFeatureChannelCount`  

The number of feature channels in the input tensor.

`outputFeatureChannelCount`  

The number of feature channels in the output tensor.

`groupCount`  

The number of groups.

`strides`  

A tuple that contains the kernel strides for y and x.

`dilationRates`  

A tuple that contains the dilation rates for y and x.

`paddingPolicy`  

The padding policy.

## See Also

### Creating Convolution Descriptors

convenience init(transposeWithKernelWidth: Int, kernelHeight: Int, inputFeatureChannelCount: Int, outputFeatureChannelCount: Int)

Creates a descriptor for convolution transpose with the kernel sizes and number of feature channels you specify.

Deprecated

convenience init(depthwiseWithKernelWidth: Int, kernelHeight: Int, inputFeatureChannelCount: Int, channelMultiplier: Int)

Creates a descriptor for depthwise convolution with the kernel sizes, number of input feature channels, and channel multiplier you specify.

Deprecated

enum MLCConvolutionType

The convolution type specified for a convolution layer.

Deprecated

