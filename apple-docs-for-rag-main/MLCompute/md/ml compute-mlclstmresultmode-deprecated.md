

- ML Compute
-  MLCLSTMResultMode Deprecated

Enumeration

# MLCLSTMResultMode

Constants that describe the result of an LSTM layer.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
enum MLCLSTMResultMode
```

## Topics

### Enumeration Cases

case output

A result mode that indicates the layer produces a single result tensor that represents the final output of the LSTM.

case outputAndStates

A result mode that indicates the layer produces three result tensors that represent the final output of the LSTM, the last hidden state, and the cell state.

var debugDescription: String

A textual description of the LSTM result mode you use for debugging.

### Initializers

init?(rawValue: UInt64)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

class MLCLSTMDescriptor

The configuration object you use to create the LSTM layer.

Deprecated

