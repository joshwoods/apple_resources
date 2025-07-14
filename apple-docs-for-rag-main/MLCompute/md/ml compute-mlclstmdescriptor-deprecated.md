

- ML Compute
-  MLCLSTMDescriptor Deprecated

Class

# MLCLSTMDescriptor

The configuration object you use to create the LSTM layer.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCLSTMDescriptor
```

## Topics

### Creating LSTM Descriptors

convenience init(inputSize: Int, hiddenSize: Int, layerCount: Int)

Creates a batch first LSTM descriptor with the input size and number of layers you specify.

convenience init(inputSize: Int, hiddenSize: Int, layerCount: Int, usesBiases: Bool, isBidirectional: Bool, dropout: Float)

Creates a batch first LSTM descriptor with bias and bidirectional options you specify.

convenience init(inputSize: Int, hiddenSize: Int, layerCount: Int, usesBiases: Bool, batchFirst: Bool, isBidirectional: Bool, dropout: Float)

Creates a batch first LSTM descriptor that allows you to indicate whether the input and output shape is batch first.

convenience init(inputSize: Int, hiddenSize: Int, layerCount: Int, usesBiases: Bool, batchFirst: Bool, isBidirectional: Bool, returnsSequences: Bool, dropout: Float)

Creates a batch first LSTM descriptor that allows you to indicate whether the layer returns output for all sequences, or output for only the last sequence.

convenience init(inputSize: Int, hiddenSize: Int, layerCount: Int, usesBiases: Bool, batchFirst: Bool, isBidirectional: Bool, returnsSequences: Bool, dropout: Float, resultMode: MLCLSTMResultMode)

Creates a descriptor with the number of features and layers, dropout, and options for use of biases, batch order, return sequences, bidirectionality, and expected tensors you specify.

### Inspecting LSTM Descriptors

var batchFirst: Bool

A Boolean that indicates whether the input and output shape is batch first.

var dropout: Float

The dropout probability.

var hiddenSize: Int

The number of features in the hidden state.

var inputSize: Int

The number of expected features in the input.

var isBidirectional: Bool

A Boolean that indicates whether the layer is bidirectional.

var layerCount: Int

The number of recurrent layers.

var resultMode: MLCLSTMResultMode

The mode that indicates whether the layer produces a single result tensor or three result tensors — final output, last hidden state, and the cell state.

var returnsSequences: Bool

A Boolean that indicates whether the layer returns output for all sequences.

var usesBiases: Bool

A Boolean that indicates whether you use bias weights.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Creating LSTM Layers

convenience init?(descriptor: MLCLSTMDescriptor, inputWeights: [MLCTensor], hiddenWeights: [MLCTensor], biases: [MLCTensor]?)

Creates an LSTM layer with the descriptor, input and hidden weights, and biases you specify.

Deprecated

convenience init?(descriptor: MLCLSTMDescriptor, inputWeights: [MLCTensor], hiddenWeights: [MLCTensor], peepholeWeights: [MLCTensor]?, biases: [MLCTensor]?)

Creates an LSTM layer with the descriptor, weights, and biases you specify.

Deprecated

convenience init?(descriptor: MLCLSTMDescriptor, inputWeights: [MLCTensor], hiddenWeights: [MLCTensor], peepholeWeights: [MLCTensor]?, biases: [MLCTensor]?, gateActivations: [MLCActivationDescriptor], outputResultActivation: MLCActivationDescriptor)

Creates an LSTM layer using the descriptor, weights, biases, gate activations, and output result activation that you specify.

Deprecated

enum MLCLSTMResultMode

Constants that describe the result of an LSTM layer.

Deprecated

