

- Metal Performance Shaders
- Convolutional Neural Network Kernels
-  MPSCNNPoolingL2NormGradient 

Class

# MPSCNNPoolingL2NormGradient

A gradient L2-norm pooling filter.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.0+macOS 10.13.4+tvOS 11.3+visionOS 1.0+

``` source
class MPSCNNPoolingL2NormGradient : MPSCNNPoolingGradient
```

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice, kernelWidth: Int, kernelHeight: Int, strideInPixelsX: Int, strideInPixelsY: Int)

## Relationships

### Inherits From

- MPSCNNPoolingGradient

## See Also

### Pooling Layers

class MPSCNNPoolingAverage

An average pooling filter.

class MPSCNNPoolingAverageGradient

A gradient average pooling filter.

class MPSCNNPoolingL2Norm

An L2-norm pooling filter.

class MPSCNNPoolingMax

A max pooling filter.

class MPSCNNDilatedPoolingMax

A dilated max pooling filter.

class MPSCNNPooling

A pooling kernel.

class MPSCNNPoolingGradient

A gradient pooling kernel.

class MPSCNNDilatedPoolingMaxGradient

A gradient dilated max pooling filter.

class MPSCNNPoolingMaxGradient

A gradient max pooling filter.

