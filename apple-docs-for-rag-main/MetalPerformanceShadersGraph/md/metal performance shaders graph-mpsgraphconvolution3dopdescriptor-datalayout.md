

- Metal Performance Shaders Graph
- MPSGraphConvolution3DOpDescriptor
-  dataLayout 

Instance Property

# dataLayout

The named layout of data in the source tensor.

iOS 16.3+iPadOS 16.3+Mac Catalyst 16.3+macOS 13.2+tvOS 16.3+visionOS 1.0+

``` source
var dataLayout: MPSGraphTensorNamedDataLayout { get set }
```

## Discussion

It defines the order of named dimensions (Batch, Channel, Depth, Height, Width). The convolution operation uses this to interpret data in the source tensor. For example, if `dataLayout` is `MPSGraphTensorNamedDataLayoutNCDHW`, frameork interprets data in source tensor as `batch x channels x depth x height x width` with `width` as fastest moving dimension.

