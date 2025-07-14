

- Metal Performance Shaders Graph
- MPSGraphConvolution3DOpDescriptor
-  weightsLayout 

Instance Property

# weightsLayout

The named layout of data in the weights tensor.

iOS 16.3+iPadOS 16.3+Mac Catalyst 16.3+macOS 13.2+tvOS 16.3+visionOS 1.0+

``` source
var weightsLayout: MPSGraphTensorNamedDataLayout { get set }
```

## Discussion

It defines the order of named dimensions (Output channels, Input channels, Kernel depth, Kernel height, Kernel width). The convolution operation uses this to interpret data in the weights tensor. For example, if `weightsLayout` is `MPSGraphTensorNamedDataLayoutOIDHW`, frameork interprets data in weights tensor as `outputChannels x inputChannels x kernelDepth x kernelHeight x kernelWidth` with `kernelWidth` as fastest moving dimension.

