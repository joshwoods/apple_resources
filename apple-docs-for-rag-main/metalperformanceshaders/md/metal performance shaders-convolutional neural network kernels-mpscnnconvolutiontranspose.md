

- Metal Performance Shaders
- Convolutional Neural Network Kernels
-  MPSCNNConvolutionTranspose 

Class

# MPSCNNConvolutionTranspose

A transposed convolution kernel.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class MPSCNNConvolutionTranspose : MPSCNNKernel
```

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

Initializes a transposed convolution kernel.

init(device: any MTLDevice, weights: any MPSCNNConvolutionDataSource)

Initializes a transposed convolution kernel.

protocol MPSCNNConvolutionDataSource

The protocol that provides convolution filter weights and bias terms.

### Instance Properties

var groups: Int

var inputFeatureChannels: Int

var kernelOffsetX: Int

var kernelOffsetY: Int

var outputFeatureChannels: Int

var accumulatorPrecisionOption: MPSNNConvolutionAccumulatorPrecisionOption

var dataSource: any MPSCNNConvolutionDataSource

### Instance Methods

func encode(commandBuffer: any MTLCommandBuffer, sourceImage: MPSImage, convolutionGradientState: MPSCNNConvolutionGradientState?) -> MPSImage

func encode(commandBuffer: any MTLCommandBuffer, sourceImage: MPSImage, convolutionGradientState: MPSCNNConvolutionGradientState?, destinationImage: MPSImage)

func encode(commandBuffer: any MTLCommandBuffer, sourceImage: MPSImage, convolutionGradientState: MPSCNNConvolutionGradientState?, destinationState: AutoreleasingUnsafeMutablePointer&lt;MPSCNNConvolutionTransposeGradientState?>, destinationStateIsTemporary: Bool) -> MPSImage

func encodeBatch(commandBuffer: any MTLCommandBuffer, sourceImages: [MPSImage], convolutionGradientStates: [MPSCNNConvolutionGradientState]?) -> [MPSImage]

func encodeBatch(commandBuffer: any MTLCommandBuffer, sourceImages: [MPSImage], convolutionGradientStates: [MPSCNNConvolutionGradientState]?, destinationImages: [MPSImage])

func encodeBatch(commandBuffer: any MTLCommandBuffer, sourceImages: [MPSImage], convolutionGradientStates: [MPSCNNConvolutionGradientState]?, destinationStates: AutoreleasingUnsafeMutablePointer&lt;NSArray?>, destinationStateIsTemporary: Bool) -> [MPSImage]

func exportWeightsAndBiases(with: any MTLCommandBuffer, resultStateCanBeTemporary: Bool) -> MPSCNNConvolutionWeightsAndBiasesState

func reloadWeightsAndBiases(with: any MTLCommandBuffer, state: MPSCNNConvolutionWeightsAndBiasesState)

func reloadWeightsAndBiasesFromDataSource()

func resultState(sourceImage: MPSImage, sourceStates: [MPSCNNConvolutionGradientState]?, destinationImage: MPSImage) -> MPSCNNConvolutionTransposeGradientState?

func resultStateBatch(sourceImage: [MPSImage], sourceStates: [[MPSCNNConvolutionGradientState]]?, destinationImage: [MPSImage]) -> [MPSCNNConvolutionTransposeGradientState]?

func temporaryResultState(commandBuffer: any MTLCommandBuffer, sourceImage: MPSImage, sourceStates: [MPSCNNConvolutionGradientState]?, destinationImage: MPSImage) -> MPSCNNConvolutionTransposeGradientState?

func temporaryResultStateBatch(commandBuffer: any MTLCommandBuffer, sourceImage: [MPSImage], sourceStates: [[MPSCNNConvolutionGradientState]]?, destinationImage: [MPSImage]) -> [MPSCNNConvolutionTransposeGradientState]?

## Relationships

### Inherits From

- MPSCNNKernel

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

class MPSCNNConvolutionGradient

A gradient convolution kernel.

class MPSCNNConvolutionGradientState

An object that exposes a gradient convolution kernel's gradient with respect to weights and biases.

protocol MPSImageSizeEncodingState

A protocol for objects that contain information about an image size elsewhere in the graph.

class MPSCNNConvolutionWeightsAndBiasesState

A class that stores weights and biases.

