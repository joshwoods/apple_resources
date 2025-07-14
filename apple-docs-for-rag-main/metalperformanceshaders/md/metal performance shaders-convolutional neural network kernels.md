

- Metal Performance Shaders
-  Convolutional Neural Network Kernels 

API Collection

# Convolutional Neural Network Kernels

Build neural networks with layers.

## Overview

- Think carefully about the edge mode requested for pooling layers. The default value is MPSImageEdgeMode.zero, but there are times when a MPSImageEdgeMode.clamp value may be better.

- To avoid reading off the edge of an image for filters that have a filter area (convolution, pooling), set `MPSCNNKernel.offset = (MPSOffset){ .x = kernelWidth/2, .y = kernelHeight/2, .z = 0}` and reduce the size of the output image by `{kernelWidth-1, kernelHeight-1, 0}`. The filter area stretches up and to the left of the kernel offset by `{kernelWidth/2, kernelHeight/2}`.

- Always remember the following distinction:

  - The MPSCNNConvolution class takes weights in the order `weight[outputChannels][kernelHeight][kernelWidth][inputChannels/groups]`.

  - The MPSCNNFullyConnected class takes weights in the order `weight[outputChannels][sourceWidth][sourceHeight][inputChannels]`.

- Initialize MPSCNNKernel objects once and reuse them.

- You can use MPSCNNNeuron objects and similar to perform pre-processing of images, such as scaling and resizing.

- Specify a neuron filter with an MPSCNNConvolutionDescriptor object to combine the convolution and neuron operations.

- Use MPSTemporaryImage objects for intermediate images that live for a short period of time (one MTLCommandBuffer object).

  MPSTemporaryImage objects can reduce the amount of memory used by the CNN by several folds, and similarly reduce the amount of CPU time spent allocating storage and latency between the time a command buffer is committed and when it is actually executed on the GPU.

  You cannot read or write to a MPSTemporaryImage object using the CPU. Generally, MPSTemporaryImage objects should be created as needed and thrown away promptly. Persistent objects should not retain them.

  Please be sure to understand the purpose of the readCount property.

- Because the Metal Performance Shaders framework encodes its work in place in your command buffer, you always have the option to insert your own code in between MPSCNNKernel encodings as a Metal function for tasks not covered by the framework. You do not need to use the Metal Performance Shaders framework for everything.

## Topics

### Arithmetic Layers

class MPSCNNAdd

An addition operator.

class MPSCNNAddGradient

A gradient addition operator.

class MPSCNNSubtract

A subtraction operator.

class MPSCNNSubtractGradient

A gradient subtraction operator.

class MPSCNNMultiply

A multiply operator.

class MPSCNNMultiplyGradient

A gradient multiply operator.

class MPSCNNDivide

A division operator.

class MPSCNNArithmetic

The base class for arithmetic operators.

class MPSCNNArithmeticGradient

The base class for gradient arithmetic operators.

class MPSCNNArithmeticGradientState

An object that stores the clamp mask used by gradient arithmetic operators.

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

protocol MPSImageSizeEncodingState

A protocol for objects that contain information about an image size elsewhere in the graph.

class MPSCNNConvolutionWeightsAndBiasesState

A class that stores weights and biases.

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

class MPSCNNPoolingL2NormGradient

A gradient L2-norm pooling filter.

class MPSCNNPoolingMaxGradient

A gradient max pooling filter.

### Fully Connected Layers

class MPSCNNBinaryFullyConnected

A fully connected convolution layer with binary weights and optionally binarized input image.

class MPSCNNFullyConnected

A fully connected convolution layer, also known as an inner product layer.

class MPSCNNFullyConnectedGradient

A gradient fully connected convolution layer.

### Neuron Layers

class MPSCNNNeuronAbsolute

An absolute neuron filter.

class MPSCNNNeuronELU

A parametric ELU neuron filter.

class MPSCNNNeuronHardSigmoid

A hard sigmoid neuron filter.

class MPSCNNNeuronLinear

A linear neuron filter.

class MPSCNNNeuronPReLU

A parametric ReLU (Rectified Linear Unit) neuron filter.

class MPSCNNNeuronReLUN

A ReLUN neuron filter.

class MPSCNNNeuronReLU

A ReLU (Rectified Linear Unit) neuron filter.

class MPSCNNNeuronSigmoid

A sigmoid neuron filter.

class MPSCNNNeuronSoftPlus

A parametric softplus neuron filter.

class MPSCNNNeuronSoftSign

A softsign neuron filter.

class MPSCNNNeuronTanH

A hyperbolic tangent neuron filter.

class MPSCNNNeuron

A filter that applies a neuron activation function.

class MPSCNNNeuronExponential

An exponential neuron filter.

class MPSCNNNeuronGradient

A gradient neuron filter.

class MPSCNNNeuronLogarithm

A logarithm neuron filter.

class MPSCNNNeuronPower

A power neuron filter.

class MPSNNNeuronDescriptor

An object that specifies properties used by a neuron kernel.

### Softmax Layers

class MPSCNNSoftMax

A neural transfer function that is useful for classification tasks.

class MPSCNNLogSoftMax

A neural transfer function that is useful for constructing a loss function to be minimized when training neural networks.

class MPSCNNLogSoftMaxGradient

A gradient logarithmic softmax filter.

class MPSCNNSoftMaxGradient

A gradient softmax filter.

### Normalization Layers

class MPSCNNCrossChannelNormalization

A normalization kernel applied across feature channels.

class MPSCNNCrossChannelNormalizationGradient

A gradient normalization kernel applied across feature channels.

class MPSCNNLocalContrastNormalization

A local-contrast normalization kernel.

class MPSCNNLocalContrastNormalizationGradient

A gradient local-contrast normalization kernel.

class MPSCNNSpatialNormalization

A spatial normalization kernel.

class MPSCNNSpatialNormalizationGradient

A gradient spatial normalization kernel.

class MPSCNNBatchNormalization

A batch normalization kernel.

class MPSCNNBatchNormalizationGradient

A gradient batch normalization kernel.

class MPSCNNBatchNormalizationState

An object that stores data required to execute batch normalization.

class MPSCNNNormalizationMeanAndVarianceState

An object that stores mean and variance terms used to execute batch normalization.

class MPSCNNBatchNormalizationStatistics

An object that stores statistics required to execute batch normalization.

class MPSCNNBatchNormalizationStatisticsGradient

An object that stores the gradient of the loss function with respect to the batch statistics and batch normalization weights.

class MPSCNNInstanceNormalization

An instance normalization kernel.

class MPSCNNInstanceNormalizationGradient

A gradient instance normalization kernel.

class MPSCNNInstanceNormalizationGradientState

An object that stores information required to execute a gradient pass for instance normalization.

class MPSCNNNormalizationGammaAndBetaState

An object that stores gamma and beta terms used to apply a scale and bias in instance- or batch-normalization operations.

### Upsampling Layers

class MPSCNNUpsampling

A filter that resamples an existing MPS image.

class MPSCNNUpsamplingBilinear

A bilinear spatial upsampling filter.

class MPSCNNUpsamplingNearest

A nearest spatial upsampling filter.

class MPSCNNUpsamplingBilinearGradient

A gradient bilinear spatial upsampling filter.

class MPSCNNUpsamplingGradient

A gradient filter that upsamples an existing Metal Performance Shaders image.

class MPSCNNUpsamplingNearestGradient

A gradient upsampling filter that samples the pixel nearest to the source when upsampling to the destination pixel.

### Dropout Layers

class MPSCNNDropout

A dropout filter.

class MPSCNNDropoutGradient

A gradient dropout filter.

class MPSCNNDropoutGradientState

A class that stores the mask used by dropout and gradient dropout filters.

### Loss Layers

class MPSCNNLoss

A kernel that computes the loss and loss gradient between specified predictions and labels.

class MPSCNNLossDataDescriptor

An object that specifies properties used by a loss data descriptor.

class MPSCNNLossDescriptor

An object that specifies properties used by a loss kernel.

class MPSCNNLossLabels

A class that stores the per-element weight buffer used by loss and gradient loss kernels.

class MPSCNNYOLOLoss

A kernel that computes the YOLO loss and loss gradient between specified predictions and labels.

class MPSCNNYOLOLossDescriptor

An object that specifies properties used by a YOLO loss kernel.

### Reduction Layers

class MPSNNReduceRowMax

A reduction filter that returns the maximum value for each row in an image.

class MPSNNReduceRowMin

A reduction filter that returns the minimum value for each row in an image.

class MPSNNReduceRowSum

A reduction filter that returns the sum of all values for each row in an image.

class MPSNNReduceRowMean

A reduction filter that returns the mean value for each row in an image.

class MPSNNReduceColumnMax

A reduction filter that returns the maximum value for each column in an image.

class MPSNNReduceColumnMin

A reduction filter that returns the minimum value for each column in an image.

class MPSNNReduceColumnSum

A reduction filter that returns the sum of all values for each column in an image.

class MPSNNReduceColumnMean

A reduction filter that returns the mean value for each column in an image.

class MPSNNReduceFeatureChannelsMax

A reduction filter that returns the maximum value for each feature channel in an image.

class MPSNNReduceFeatureChannelsMin

A reduction filter that returns the minimum value for each feature channel in an image.

class MPSNNReduceFeatureChannelsSum

A reduction filter that returns the sum of all values for each feature channel in an image.

class MPSNNReduceFeatureChannelsMean

A reduction filter that returns the mean value for each feature channel in an image.

class MPSNNReduceFeatureChannelsArgumentMax

A reduction filter that returns the index of the location of the maximum value for each feature channel in an image.

class MPSNNReduceFeatureChannelsArgumentMin

A reduction filter that returns the index of the location of the minimum value for each feature channel in an image.

class MPSNNReduceFeatureChannelsAndWeightsSum

A reduction filter that returns the weighted sum of all values for each feature channel in an image.

class MPSNNReduceFeatureChannelsAndWeightsMean

A reduction filter that returns the weighted sum for each feature channel in an image.

class MPSNNReduceUnary

The base class for unary reduction filters.

class MPSNNReduceBinary

The base class for binary reduction filters.

### Reshape Layer

class MPSNNReshape

The base class for reshape operations.

### Slice Layer

class MPSNNSlice

A kernel that extracts a slice from an image.

### Optimization Layers

class MPSNNOptimizerAdam

An optimization layer that performs an Adam pdate.

class MPSNNOptimizerRMSProp

An optimization layer that performs a root mean square propagation update.

class MPSNNOptimizerStochasticGradientDescent

An optimization layer that performs a gradient descent with an optional momentum update.

class MPSNNOptimizer

The base class for optimization layers.

class MPSNNOptimizerDescriptor

An object that specifies properties used by an optimizer kernel.

### Layer Base Classes

class MPSCNNKernel

Base class for neural network layers.

class MPSCNNBinaryKernel

A convolution neural network kernel.

class MPSCNNGradientKernel

The base class for gradient layers.

### Predefined Padding Policies

class MPSNNDefaultPadding

A class that provides predefined padding policies for common tasks.

## See Also

### Neural Networks

Training a Neural Network with Metal Performance Shaders

Use an MPS neural network graph to train a simple neural network digit classifier.

class MPSImage

A texture that may have more than four channels for use in convolutional neural networks.

class MPSTemporaryImage

A texture for use in convolutional neural networks that stores transient data to be used and discarded promptly.

Objects that Simplify the Creation of Neural Networks

Simplify the creation of neural networks using networks of filter, image, and state nodes.

Recurrent Neural Networks

Create recurrent neural networks.

