

- Metal Performance Shaders
- Convolutional Neural Network Kernels
-  MPSCNNDilatedPoolingMaxGradient 

Class

# MPSCNNDilatedPoolingMaxGradient

A gradient dilated max pooling filter.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.0+macOS 10.13.4+tvOS 11.3+visionOS 1.0+

``` source
class MPSCNNDilatedPoolingMaxGradient : MPSCNNPoolingGradient
```

## Overview

A gradient max pooling filter but the pixels selected in each “application” of the max pooling operation are exactly the same pixels that would be selected with dilated convolution

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice, kernelWidth: Int, kernelHeight: Int, dilationRateX: Int, dilationRateY: Int, strideInPixelsX: Int, strideInPixelsY: Int)

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

class MPSCNNPoolingL2NormGradient

A gradient L2-norm pooling filter.

class MPSCNNPoolingMaxGradient

A gradient max pooling filter.

