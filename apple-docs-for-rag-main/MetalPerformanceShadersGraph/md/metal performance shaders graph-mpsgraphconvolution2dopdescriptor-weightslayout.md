

- Metal Performance Shaders Graph
- MPSGraphConvolution2DOpDescriptor
-  weightsLayout 

Instance Property

# weightsLayout

The named layout of data in the weights tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var weightsLayout: MPSGraphTensorNamedDataLayout { get set }
```

## Discussion

It defines the order of named dimensions (Output channels, Input channels, Kernel height, Kernel width). The convolution operation uses this to interpret data in the weights tensor. For example, if `weightsLayout` is `MPSGraphTensorNamedDataLayoutOIHW`, frameork interprets data in weights tensor as `outputChannels x inputChannels x kernelHeight x kernelWidth` with `kernelWidth` as fastest moving dimension.

