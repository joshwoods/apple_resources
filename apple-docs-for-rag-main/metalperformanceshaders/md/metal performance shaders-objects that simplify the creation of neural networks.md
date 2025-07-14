

- Metal Performance Shaders
-  Objects that Simplify the Creation of Neural Networks 

API Collection

# Objects that Simplify the Creation of Neural Networks

Simplify the creation of neural networks using networks of filter, image, and state nodes.

## Overview

Graphs in Metal Performance Shaders offer a higher level graph API, intended to simplify the creation of neural networks. The graph is a network of MPSNNFilterNode, MPSNNImageNode and MPSNNStateNode objects.

- `MPSNNImageNode` represents MPSImage or MPSTemporaryImage objects

- `MPSNNFilterNode` represents MPSCNNKernel objects—each of the lower level `MPSCNNKernel` subclasses has an associated object that is a subclass of the `MPSNNFilterNode`

- `MPSNNStateNode` represents MPSState objects

## Topics

### Neural Network Graphs

class MPSNNGraph

An optimized representation of a graph of neural network image and filter nodes.

class MPSNNImageNode

A placeholder node denoting the position of a neural network image in a graph.

protocol MPSHandle

The protocol that provides resource identification.

### Arithmetic Layer Nodes

class MPSNNAdditionNode

A representation of an addition operator.

class MPSNNAdditionGradientNode

A representation of a gradient addition operator.

class MPSNNSubtractionNode

A representation of an subtraction operator.

class MPSNNSubtractionGradientNode

A representation of a gradient subtraction operator.

class MPSNNMultiplicationNode

A representation of a multiplication operator.

class MPSNNMultiplicationGradientNode

A representation of a gradient multiplication operator.

class MPSNNDivisionNode

A representation of a division operator.

class MPSNNBinaryArithmeticNode

Virtual base class for basic arithmetic nodes.

class MPSNNArithmeticGradientNode

A representation of the base class for gradient arithmetic operators.

class MPSNNArithmeticGradientStateNode

A representation of the clamp mask used by gradient arithmetic operators.

### Convolution Layer Nodes

class MPSCNNBinaryConvolutionNode

A representation of a convolution kernel with binary weights and an input image using binary approximations.

class MPSCNNConvolutionNode

A representation of a convolution kernel.

class MPSCNNConvolutionTransposeNode

A representation of a transposed convolution.

class MPSCNNConvolutionGradientNode

A representation of a gradient convolution kernel.

class MPSCNNConvolutionGradientStateNode

A representation of a gradient convolution state.

class MPSCNNCrossChannelNormalizationGradientNode

A representation of a gradient normalization kernel applied across feature channels.

### Pooling Layer Nodes

class MPSCNNPoolingAverageNode

A representation of an average pooling filter.

class MPSCNNDilatedPoolingMaxNode

A representation of a dilated max pooling filter.

class MPSCNNPoolingL2NormNode

A representation of a L2-norm pooling filter.

class MPSCNNPoolingMaxNode

A representation of a max pooling filter.

class MPSCNNPoolingNode

A representation of a MPS CNN pooling kernel.

class MPSCNNDilatedPoolingMaxGradientNode

A representation of a gradient dilated max pooling filter.

class MPSCNNPoolingAverageGradientNode

A representation of a gradient average pooling filter.

class MPSCNNPoolingGradientNode

A representation of a gradient pooling kernel.

class MPSCNNPoolingL2NormGradientNode

A representation of a gradient L2-norm pooling filter.

class MPSCNNPoolingMaxGradientNode

A representation of a gradient max pooling filter.

### Fully Connected Layer Nodes

class MPSCNNBinaryFullyConnectedNode

A representation of a fully connected convolution layer with binary weights and optionally binarized input image.

class MPSCNNFullyConnectedNode

A representation of a fully connected convolution layer, also known as an inner product layer.

### Neuron Layer Nodes

class MPSCNNNeuronAbsoluteNode

A representation of an absolute neuron filter.

class MPSCNNNeuronELUNode

A representation of a parametric ELU neuron filter.

class MPSCNNNeuronHardSigmoidNode

A representation of a hard sigmoid neuron filter.

class MPSCNNNeuronLinearNode

A representation of a linear neuron filter.

class MPSCNNNeuronPReLUNode

A representation a PReLU neuron filter.

class MPSCNNNeuronReLUNNode

A representation a ReLUN neuron filter.

class MPSCNNNeuronReLUNode

A representation a ReLU neuron filter.

class MPSCNNNeuronSigmoidNode

A representation of a sigmoid neuron filter.

class MPSCNNNeuronSoftPlusNode

A representation of a parametric softplus neuron filter.

class MPSCNNNeuronSoftSignNode

A representation of a softsign neuron filter.

class MPSCNNNeuronTanHNode

A representation of a hyperbolic tangent neuron filter.

class MPSCNNNeuronExponentialNode

A representation of an exponential neuron filter.

class MPSCNNNeuronGradientNode

A representation of a gradient exponential neuron filter.

class MPSCNNNeuronLogarithmNode

A representation of a logarithm neuron filter.

class MPSCNNNeuronPowerNode

A representation of a power neuron filter.

class MPSCNNNeuronNode

The virtual base class for MPS CNN neuron nodes.

### Softmax Layer Nodes

class MPSCNNSoftMaxNode

A representation of a softmax filter.

class MPSCNNLogSoftMaxNode

A representation of a logarithmic softmax filter kernel.

class MPSCNNLogSoftMaxGradientNode

A representation of a gradient logarithmic softmax filter kernel.

class MPSCNNSoftMaxGradientNode

A representation of a gradient softmax filter.

### Normalization Layer Nodes

class MPSCNNCrossChannelNormalizationNode

A representation of a normalization kernel across feature channels.

class MPSCNNLocalContrastNormalizationNode

A representation of a local-contrast normalization kernel.

class MPSCNNSpatialNormalizationNode

A representation of a spatial normalization kernel.

class MPSCNNBatchNormalizationGradientNode

A representation of a gradient batch normalization kernel.

class MPSCNNBatchNormalizationNode

A representation of a batch normalization kernel.

protocol MPSCNNBatchNormalizationDataSource

A protocol that defines methods that a batch normalization state uses to initialize scale factors, bias terms, and batch statistics.

class MPSCNNInstanceNormalizationGradientNode

A representation of a gradient instance normalization kernel.

protocol MPSCNNInstanceNormalizationDataSource

A protocol that defines methods that an instance normalization uses to initialize scale factors and bias terms.

class MPSCNNInstanceNormalizationNode

A representation of an instance normalization kernel.

class MPSCNNLocalContrastNormalizationGradientNode

A representation of a gradient local-contrast normalization kernel.

class MPSCNNSpatialNormalizationGradientNode

A representation of a gradient spatial normalization kernel.

class MPSCNNNormalizationNode

Virtual base class for CNN normalization nodes.

### Upsampling Layer Nodes

class MPSCNNUpsamplingBilinearNode

A representation of a bilinear spatial upsampling filter.

class MPSCNNUpsamplingNearestNode

A representation of a nearest spatial upsampling filter.

class MPSCNNUpsamplingBilinearGradientNode

A representation of a gradient bilinear spatial upsampling filter.

class MPSCNNUpsamplingNearestGradientNode

A representation of a gradient nearest spatial upsampling filter.

### Resampling Nodes

class MPSNNBilinearScaleNode

A representation of a bilinear resampling filter.

class MPSNNLanczosScaleNode

A representation of a Lanczos resampling filter.

class MPSNNScaleNode

Abstract node representing an image resampling filter.

protocol MPSImageTransformProvider

A general interface for objects that provide image resampling.

### Dropout Layer Nodes

class MPSCNNDropoutNode

A representation of a dropout filter.

class MPSCNNDropoutGradientNode

A representation of a gradient dropout filter.

### Kernel Concatenation Nodes

class MPSNNConcatenationNode

A representation of the results from one or more kernels.

class MPSNNConcatenationGradientNode

A representation of the results from one or more gradient kernels.

### Loss Layer Nodes

class MPSCNNLossNode

A representation of a loss kernel.

class MPSCNNYOLOLossNode

A representation of a YOLO loss kernel.

class MPSNNLabelsNode

A placeholder node denoting the per-element weight buffer used by loss and gradient loss kernels.

### Filter Node Base Classes

class MPSNNFilterNode

A placeholder node denoting a neural network filter stage.

class MPSNNGradientFilterNode

A representation of a gradient filter.

### Protocols

protocol MPSNNTrainableNode

A protocol that defines methods that determine whether and when neural network training parameters are updated.

## See Also

### Neural Networks

Training a Neural Network with Metal Performance Shaders

Use an MPS neural network graph to train a simple neural network digit classifier.

class MPSImage

A texture that may have more than four channels for use in convolutional neural networks.

class MPSTemporaryImage

A texture for use in convolutional neural networks that stores transient data to be used and discarded promptly.

Convolutional Neural Network Kernels

Build neural networks with layers.

Recurrent Neural Networks

Create recurrent neural networks.

