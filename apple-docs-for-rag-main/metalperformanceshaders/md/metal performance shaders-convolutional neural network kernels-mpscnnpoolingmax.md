

- Metal Performance Shaders
- Convolutional Neural Network Kernels
-  MPSCNNPoolingMax 

Class

# MPSCNNPoolingMax

A max pooling filter.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
class MPSCNNPoolingMax : MPSCNNPooling
```

## Overview

For each pixel in an image, the filter returns the maximum value of the pixels in the filter region defined by `kernelWidth` x `kernelHeight`.

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

Initializes a max pooling filter.

init(device: any MTLDevice, kernelWidth: Int, kernelHeight: Int, strideInPixelsX: Int, strideInPixelsY: Int)

Initializes a max pooling filter.

## Relationships

### Inherits From

- MPSCNNPooling

## See Also

### Pooling Layers

class MPSCNNPoolingAverage

An average pooling filter.

class MPSCNNPoolingAverageGradient

A gradient average pooling filter.

class MPSCNNPoolingL2Norm

An L2-norm pooling filter.

class MPSCNNDilatedPoolingMax

A dilated max pooling filter.

class MPSCNNPooling

A pooling kernel.

class MPSCNNPoolingGradient

A gradient pooling kernel.

class MPSCNNDilatedPoolingMaxGradient

A gradient dilated max pooling filter.

class MPSCNNPoolingL2NormGradient

A gradient L2-norm pooling filter.

class MPSCNNPoolingMaxGradient

A gradient max pooling filter.

