

- Metal Performance Shaders
- Convolutional Neural Network Kernels
-  MPSImageSizeEncodingState 

Protocol

# MPSImageSizeEncodingState

A protocol for objects that contain information about an image size elsewhere in the graph.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
protocol MPSImageSizeEncodingState
```

## Topics

### Instance Properties

var sourceHeight: Int

**Required**

var sourceWidth: Int

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- MPSCNNConvolutionGradientState

## See Also

### Convolution Layers

class MPSCNNBinaryConvolution

A convolution kernel with binary weights and an input image using binary approximations.

class MPSCNNConvolution

A convolution kernel that convolves the input image with a set of filters, with each producing one feature map in the output image.

class MPSCNNDepthWiseConvolutionDescriptor

A description of a convolution object that does depthwise convolution.

class MPSCNNSubPixelConvolutionDescriptor

A description of a convolution object that does subpixel upsampling and reshaping.

class MPSCNNConvolutionTranspose

A transposed convolution kernel.

class MPSCNNConvolutionGradient

A gradient convolution kernel.

class MPSCNNConvolutionGradientState

An object that exposes a gradient convolution kernel's gradient with respect to weights and biases.

class MPSCNNConvolutionWeightsAndBiasesState

A class that stores weights and biases.

