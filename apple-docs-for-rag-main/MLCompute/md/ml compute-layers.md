

- ML Compute
-  Layers 

API Collection

# Layers

Create and inspect layers that encapsulate operations and configuration details to receive, process, and output tensors.

## Topics

### Activation Layers

class MLCActivationLayer

A layer that applies an activation function to the source tensor and produces an output.

Deprecated

class MLCMultiheadAttentionLayer

A multihead, scaled dot-product attention layer that attends to one or more entries in the input key-value pairs.

Deprecated

class MLCSoftmaxLayer

A layer that outputs a probability distribution as attention weights.

Deprecated

### Math Layers

class MLCArithmeticLayer

A layer that performs an arithmetic operation.

Deprecated

class MLCReductionLayer

A layer that reduces tensor values across a specific dimension to a scalar value.

Deprecated

class MLCMatMulLayer

A layer that multiplies matrices.

Deprecated

class MLCFullyConnectedLayer

A layer that connects each input to each output within its layer.

Deprecated

class MLCGramMatrixLayer

A layer that computes the uncentered cross-correlation values between the spacial planes of each feature channel of a tensor.

Deprecated

class MLCComparisonLayer

A layer that performs elementwise comparison of two tensors.

Deprecated

### Transformation Layers

class MLCTransposeLayer

A layer that permutes the dimensions you specify.

Deprecated

class MLCConcatenationLayer

A layer that combines tensors into a single tensor.

Deprecated

class MLCReshapeLayer

A layer that reshapes a tensor with the shape you specify.

Deprecated

class MLCSliceLayer

A layer that extracts a slice from a tensor.

Deprecated

class MLCSplitLayer

A layer that splits a tensor value into a list of subtensors.

Deprecated

class MLCPaddingLayer

A layer that pads a tensor with the padding sizes you specify.

Deprecated

class MLCScatterLayer

A layer that updates the output at an index you specify.

Deprecated

class MLCSelectionLayer

A layer for selecting elements from two tensors.

Deprecated

class MLCGatherLayer

A layer that fetches data at the locations you specify.

Deprecated

### Normalization Layers

class MLCLayerNormalizationLayer

A layer that applies layer normalization over inputs.

Deprecated

class MLCBatchNormalizationLayer

A layer that normalizes a batch of inputs.

Deprecated

class MLCGroupNormalizationLayer

A layer that divides the channels into groups for normalization.

Deprecated

class MLCInstanceNormalizationLayer

A layer that normalizes all features of one channel.

Deprecated

class MLCDropoutLayer

A layer that deactivates neurons randomly to avoid overfitting.

Deprecated

### Convolution and Recurrent Layers

class MLCConvolutionLayer

A layer that applies a convolution over a signal.

Deprecated

class MLCLSTMLayer

A layer that represents long short-term memory (LSTM) networks.

Deprecated

class MLCPoolingLayer

A layer that summarizes the average presence of a feature.

Deprecated

class MLCUpsampleLayer

A layer that applies upsampling with the shape you specify.

Deprecated

class MLCEmbeddingLayer

A layer that stores a word embedding.

Deprecated

### Loss Layers

class MLCLossLayer

A layer that estimates the inaccuracies of the model to reduce the loss on the next evaluation.

Deprecated

class MLCYOLOLossLayer

A layer that estimates loss for the YOLO algorithm.

Deprecated

### Base Layer

class MLCLayer

The base class for all framework layers.

Deprecated

### Supporting Types

enum MLCPaddingPolicy

A padding policy that you specify for a convolution or pooling layer.

Deprecated

enum MLCPaddingType

A padding type that you specify for a padding layer.

Deprecated

## See Also

### Components

class MLCTensor

The data object you use throughout the framework.

Deprecated

class MLCPlatform

A utility class for setting global properties in the framework.

Deprecated

Training and Validation

Create, train, and validate a graph to produce acceptable prediction results.

