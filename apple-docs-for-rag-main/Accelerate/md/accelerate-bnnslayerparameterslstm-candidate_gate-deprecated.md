

- Accelerate
- BNNSLayerParametersLSTM
-  candidate_gate Deprecated

Instance Property

# candidate_gate

The descriptor of the candidate gate, which uses default tanh activation.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
var candidate_gate: BNNSLSTMGateDescriptor
```

Deprecated

Use BNNSGraph\* APIs

## Discussion

Use C style multidimensional array notation to order the memory pointers as ``` [ ``/Accelerate/BNNSLayerParametersLSTM/num_layers`` ][num_directions][ ``/Accelerate/BNNSLayerParametersLSTM/hidden_size`` ][ ``/Accelerate/BNNSLayerParametersLSTM/input_size`` / ``/Accelerate/BNNSLayerParametersLSTM/hidden_size`` ] ```.

If lstm_flags includes BNNSLayerFlagsLSTMBidirectional, BNNS defines `num_directions` as `2`, or otherwise `1`.

## See Also

### Instance Properties

var input_size: Int

The number of elements in the input.

Deprecated

var hidden_size: Int

The number of elements in the hidden state.

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

var output_gate: BNNSLSTMGateDescriptor

The descriptor of the output gate, which uses default sigmoid activation.

Deprecated

var hidden_activation: BNNSActivation

Hidden activation function, which uses default tanh activation.

Deprecated

