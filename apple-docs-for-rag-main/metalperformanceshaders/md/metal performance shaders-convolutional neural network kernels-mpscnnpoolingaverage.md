

- Metal Performance Shaders
- Convolutional Neural Network Kernels
-  MPSCNNPoolingAverage 

Class

# MPSCNNPoolingAverage

An average pooling filter.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
class MPSCNNPoolingAverage : MPSCNNPooling
```

## Overview

For each pixel in an image, the filter returns the average value of the pixels in the filter region defined by `kernelWidth`` x ``kernelHeight`.

When the value of the edgeMode property is set to MPSImageEdgeMode.clamp, the filtering window is shrunk to remain within the source image borders. For pixels close to the image borders, the filtering window will be smaller in order to fit inside the source image and less values will be used to compute the average value. In case the filtering window is entirely outside the source image border, the output value will be `0`.

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

Initializes an average pooling filter.

init(device: any MTLDevice, kernelWidth: Int, kernelHeight: Int, strideInPixelsX: Int, strideInPixelsY: Int)

Initializes an average pooling filter.

### Instance Properties

var zeroPadSizeX: Int

var zeroPadSizeY: Int

## Relationships

### Inherits From

- MPSCNNPooling

## See Also

### Pooling Layers

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

class MPSCNNPoolingL2NormGradient

A gradient L2-norm pooling filter.

class MPSCNNPoolingMaxGradient

A gradient max pooling filter.

