

- Accelerate
- BNNSLayerParametersLSTM
-  hidden_size Deprecated

Instance Property

# hidden_size

The number of elements in the hidden state.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
var hidden_size: Int
```

Deprecated

Use BNNSGraph\* APIs

## Discussion

If you set this value to a nonzero value that doesn’t match the corresponding array descriptor’s size, BNNS throws an error.

## See Also

### Instance Properties

var input_size: Int

The number of elements in the input.

Deprecated

var batch_size: Int

The number of input and output samples.

Deprecated

var num_layers: Int

The number of stacked long short-term memory (LSTM) layers.

Deprecated

var seq_len: Int

The size of the sequential input.

Deprecated

var dropout: Float

The dropout ratio to apply between long short-term memory (LSTM) layers.

Deprecated

var lstm_flags: UInt32

Flags that control the behavior of a long short-term memory (LSTM) layer.

Deprecated

var sequence_descriptor: BNNSNDArrayDescriptor

A 1D array of unsigned-integer elements that determines the batch size for each step.

Deprecated

var input_descriptor: BNNSLSTMDataDescriptor

Descriptors of the input, hidden input, and cell-state input data.

Deprecated

var output_descriptor: BNNSLSTMDataDescriptor

Descriptors of the output, hidden output, and cell-state output data.

Deprecated

var input_gate: BNNSLSTMGateDescriptor

The descriptor of the input gate, which uses default sigmoid activation.

Deprecated

var forget_gate: BNNSLSTMGateDescriptor

The descriptor of the forget gate, which uses default sigmoid activation.

Deprecated

var candidate_gate: BNNSLSTMGateDescriptor

The descriptor of the candidate gate, which uses default tanh activation.

Deprecated

var output_gate: BNNSLSTMGateDescriptor

The descriptor of the output gate, which uses default sigmoid activation.

Deprecated

var hidden_activation: BNNSActivation

Hidden activation function, which uses default tanh activation.

Deprecated

