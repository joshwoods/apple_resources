

- ML Compute
-  MLCLSTMLayer Deprecated

Class

# MLCLSTMLayer

A layer that represents long short-term memory (LSTM) networks.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCLSTMLayer
```

## Overview

Use this class to create an LSTM layer with one of the following configurations:

Unidirectional single layer  
The input weights, hidden weights, and biases are arrays of 4 tensors that describe the specified weights for the input, hidden, cell, and output gates.

Unidirectional stacked layers  
The input weights, hidden weights and biases are arrays of layerCount `* 4` tensors that describe the specified weights for the input, hidden, cell, and output gates, for `layer0...layer(layerCount - 1)`.

Bidirectional single layer  
The input weights, hidden weights, and biases are arrays of 8 tensors, where the backward time weights and biases follow the forward time weights.

## Topics

### Creating LSTM Layers

convenience init?(descriptor: MLCLSTMDescriptor, inputWeights: [MLCTensor], hiddenWeights: [MLCTensor], biases: [MLCTensor]?)

Creates an LSTM layer with the descriptor, input and hidden weights, and biases you specify.

convenience init?(descriptor: MLCLSTMDescriptor, inputWeights: [MLCTensor], hiddenWeights: [MLCTensor], peepholeWeights: [MLCTensor]?, biases: [MLCTensor]?)

Creates an LSTM layer with the descriptor, weights, and biases you specify.

convenience init?(descriptor: MLCLSTMDescriptor, inputWeights: [MLCTensor], hiddenWeights: [MLCTensor], peepholeWeights: [MLCTensor]?, biases: [MLCTensor]?, gateActivations: [MLCActivationDescriptor], outputResultActivation: MLCActivationDescriptor)

Creates an LSTM layer using the descriptor, weights, biases, gate activations, and output result activation that you specify.

class MLCLSTMDescriptor

The configuration object you use to create the LSTM layer.

enum MLCLSTMResultMode

Constants that describe the result of an LSTM layer.

### Inspecting LSTM Layers

var descriptor: MLCLSTMDescriptor

The configuration object you use to create the LSTM layer.

var gateActivations: [MLCActivationDescriptor]

The array of gate activations you use for input, hidden, cell, and output gates.

var outputResultActivation: MLCActivationDescriptor

The output activation descriptor.

var inputWeights: [MLCTensor]

The array of tensors that describe the input weights you use for the input, hidden, cell, and output gates.

var hiddenWeights: [MLCTensor]

The array of tensors that describe the hidden weights you use for the input, hidden, cell, and output gates.

var peepholeWeights: [MLCTensor]?

The array of tensors that describe the peephole weights you use for the input, hidden, cell, and output gates.

var biases: [MLCTensor]?

The array of tensors that describe the bias terms you use for the input, hidden, cell, and output gates.

var inputWeightsParameters: [MLCTensorParameter]

The input weights tensor parameters you use for optimizer updates.

var hiddenWeightsParameters: [MLCTensorParameter]

The hidden weights tensor parameters you use for optimizer updates.

var peepholeWeightsParameters: [MLCTensorParameter]?

The peephole weights tensor parameters you use for optimizer updates.

var biasesParameters: [MLCTensorParameter]?

The biases tensor parameters you use for optimizer updates.

## Relationships

### Inherits From

- MLCLayer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Convolution and Recurrent Layers

class MLCConvolutionLayer

A layer that applies a convolution over a signal.

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

