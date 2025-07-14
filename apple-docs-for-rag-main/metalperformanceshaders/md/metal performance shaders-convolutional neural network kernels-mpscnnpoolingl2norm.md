

- Metal Performance Shaders
- Convolutional Neural Network Kernels
-  MPSCNNPoolingL2Norm 

Class

# MPSCNNPoolingL2Norm

An L2-norm pooling filter.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MPSCNNPoolingL2Norm : MPSCNNPooling
```

## Overview

For each pixel, returns L2-Norm of pixels in the `kernelWidth * kernelHeight` filter region:

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

Initializes an L2-norm pooling filter.

init(device: any MTLDevice, kernelWidth: Int, kernelHeight: Int, strideInPixelsX: Int, strideInPixelsY: Int)

Initializes an L2-norm pooling filter.

## Relationships

### Inherits From

- MPSCNNPooling

## See Also

### Pooling Layers

class MPSCNNPoolingAverage

An average pooling filter.

class MPSCNNPoolingAverageGradient

A gradient average pooling filter.

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

class MPSCNNPoolingL2NormGradient

A gradient L2-norm pooling filter.

class MPSCNNPoolingMaxGradient

A gradient max pooling filter.

