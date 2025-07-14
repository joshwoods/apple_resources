

- Metal Performance Shaders
- Convolutional Neural Network Kernels
-  MPSCNNConvolutionGradient 

Class

# MPSCNNConvolutionGradient

A gradient convolution kernel.

iOS 11.3+iPadOS 11.3+Mac Catalyst 13.0+macOS 10.13.4+tvOS 11.3+visionOS 1.0+

``` source
class MPSCNNConvolutionGradient : MPSCNNGradientKernel
```

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice, weights: any MPSCNNConvolutionDataSource)

### Instance Properties

var channelMultiplier: Int

var dataSource: any MPSCNNConvolutionDataSource

var gradientOption: MPSCNNConvolutionGradientOption

var groups: Int

var serializeWeightsAndBiases: BoolDeprecated

var sourceGradientFeatureChannels: Int

var sourceImageFeatureChannels: Int

### Instance Methods

func reloadWeightsAndBiases(with: any MTLCommandBuffer, state: MPSCNNConvolutionWeightsAndBiasesState)

func reloadWeightsAndBiasesFromDataSource()

## Relationships

### Inherits From

- MPSCNNGradientKernel

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

class MPSCNNConvolutionGradientState

An object that exposes a gradient convolution kernel's gradient with respect to weights and biases.

protocol MPSImageSizeEncodingState

A protocol for objects that contain information about an image size elsewhere in the graph.

class MPSCNNConvolutionWeightsAndBiasesState

A class that stores weights and biases.

