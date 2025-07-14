

- Metal Performance Shaders
- Convolutional Neural Network Kernels
-  MPSCNNConvolution 

Class

# MPSCNNConvolution

A convolution kernel that convolves the input image with a set of filters, with each producing one feature map in the output image.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.0+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
class MPSCNNConvolution : MPSCNNKernel
```

## Overview

The attributes of a convolution operation are described by an MPSCNNConvolutionDescriptor object.

## Topics

### Initializers

init?(coder: NSCoder, device: any MTLDevice)

init(device: any MTLDevice, convolutionDescriptor: MPSCNNConvolutionDescriptor, kernelWeights: UnsafePointer&lt;Float>, biasTerms: UnsafePointer&lt;Float>?, flags: MPSCNNConvolutionFlags)

Initializes a convolution kernel.

class MPSCNNConvolutionDescriptor

A description of the attributes of a convolution kernel.

enum MPSCNNConvolutionFlags

Options used to control how kernel weights are stored and used in the CNN kernels

init(device: any MTLDevice, weights: any MPSCNNConvolutionDataSource)

protocol MPSCNNConvolutionDataSource

The protocol that provides convolution filter weights and bias terms.

### Instance Properties

var inputFeatureChannels: Int

The number of feature channels per pixel in the input image.

var outputFeatureChannels: Int

The number of feature channels per pixel in the output image.

var groups: Int

The number of groups that the input and output channels are divided into.

var subPixelScaleFactor: Int

var neuron: MPSCNNNeuron?

The neuron filter to be applied as part of the convolution operation.

class MPSCNNNeuron

A filter that applies a neuron activation function.

var neuronType: MPSCNNNeuronTypeDeprecated

enum MPSCNNNeuronType

The types of neuron filter to append to a convolution.

var neuronParameterA: FloatDeprecated

var neuronParameterB: FloatDeprecated

var accumulatorPrecisionOption: MPSNNConvolutionAccumulatorPrecisionOption

var channelMultiplier: Int

var dataSource: any MPSCNNConvolutionDataSource

var fusedNeuronDescriptor: MPSNNNeuronDescriptor?

var neuronParameterC: FloatDeprecated

### Instance Methods

func exportWeightsAndBiases(with: any MTLCommandBuffer, resultStateCanBeTemporary: Bool) -> MPSCNNConvolutionWeightsAndBiasesState

func reloadWeightsAndBiases(with: any MPSCNNConvolutionDataSource)Deprecated

func reloadWeightsAndBiases(with: any MTLCommandBuffer, state: MPSCNNConvolutionWeightsAndBiasesState)

func reloadWeightsAndBiasesFromDataSource()

func resultState(sourceImage: MPSImage, sourceStates: [MPSState]?, destinationImage: MPSImage) -> MPSCNNConvolutionGradientState?

func resultStateBatch(sourceImage: [MPSImage], sourceStates: [[MPSState]]?, destinationImage: [MPSImage]) -> [MPSCNNConvolutionGradientState]?

func temporaryResultState(commandBuffer: any MTLCommandBuffer, sourceImage: MPSImage, sourceStates: [MPSState]?, destinationImage: MPSImage) -> MPSCNNConvolutionGradientState?

func temporaryResultStateBatch(commandBuffer: any MTLCommandBuffer, sourceImage: [MPSImage], sourceStates: [[MPSState]]?, destinationImage: [MPSImage]) -> [MPSCNNConvolutionGradientState]?

## Relationships

### Inherits From

- MPSCNNKernel

## See Also

### Convolution Layers

class MPSCNNBinaryConvolution

A convolution kernel with binary weights and an input image using binary approximations.

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

protocol MPSImageSizeEncodingState

A protocol for objects that contain information about an image size elsewhere in the graph.

class MPSCNNConvolutionWeightsAndBiasesState

A class that stores weights and biases.

