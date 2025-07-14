

- Accelerate
- BNNSLayerParametersLSTM
-  init(input_size:hidden_size:batch_size:num_layers:seq_len:dropout:lstm_flags:sequence_descriptor:input_descriptor:output_descriptor:input_gate:forget_gate:candidate_gate:output_gate:hidden_activation:) Deprecated

Initializer

# init(input_size:hidden_size:batch_size:num_layers:seq_len:dropout:lstm_flags:sequence_descriptor:input_descriptor:output_descriptor:input_gate:forget_gate:candidate_gate:output_gate:hidden_activation:)

Returns a new long short-term memory (LSTM) parameters structure from the specified parameters.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init(
    input_size: Int,
    hidden_size: Int,
    batch_size: Int,
    num_layers: Int,
    seq_len: Int,
    dropout: Float,
    lstm_flags: UInt32,
    sequence_descriptor: BNNSNDArrayDescriptor,
    input_descriptor: BNNSLSTMDataDescriptor,
    output_descriptor: BNNSLSTMDataDescriptor,
    input_gate: BNNSLSTMGateDescriptor,
    forget_gate: BNNSLSTMGateDescriptor,
    candidate_gate: BNNSLSTMGateDescriptor,
    output_gate: BNNSLSTMGateDescriptor,
    hidden_activation: BNNSActivation
)
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`input_size`  

The number of elements in the input.

`hidden_size`  

The number of elements in the hidden state.

`batch_size`  

The number of input and output samples.

`num_layers`  

The number of stacked LSTM layers.

`seq_len`  

The size of the sequential input.

`dropout`  

The dropout ratio to apply between LSTM layers. BNNS doesn’t apply dropout to the last stacked layer and ignores this parameter when the number of layers is `1`.

`lstm_flags`  

Flags that control the behavior of an LSTM layer.

`sequence_descriptor`  

A 1D array of unsigned-integer elements that determines the batch size for each step. If seq_len is greater than `1` and the data property of this descriptor is `nil`, BNNS uses the same batch_size for the entire sequence.

`input_descriptor`  

Descriptors of the input, hidden input, and cell-state input data. For more information, see input_descriptor.

`output_descriptor`  

Descriptors of the output, hidden output, and cell-state output data. For more information, see output_descriptor.

`input_gate`  

The descriptor of the input gate, which uses default sigmoid activation. Use C style multidimensional array notation to order the memory pointers as `[num_layers][num_directions][hidden_size][input_size/hidden_size]`.

`forget_gate`  

The descriptor of the forget gate, which uses default sigmoid activation. Use C style multidimensional array notation to order the memory pointers as `[num_layers][num_directions][hidden_size][input_size/hidden_size]`.

`candidate_gate`  

The descriptor of the candidate gate, which uses default tanh activation. Use C style multidimensional array notation to order the memory pointers as `[num_layers][num_directions][hidden_size][input_size/hidden_size]`.

`output_gate`  

The descriptor of the output gate, which uses default sigmoid activation. Use C style multidimensional array notation to order the memory pointers as `[num_layers][num_directions][hidden_size][input_size/hidden_size]`.

`hidden_activation`  

Hidden activation function, which uses default tanh activation.

## Discussion

To enable peephole connections, set the weights pointer in the corresponding gates descriptor. To enable bias, set the bias pointer in the corresponding gates descriptor.

BNNS treats the hidden_desc of the input_descriptor as a zero-filled array if its data is `nil`. BNNS treats the cell_state_desc of the input_descriptor as a zero-filled array if its data is `nil`.

## See Also

### Initializers

init()

Returns a new long short-term memory (LSTM) parameters structure.

Deprecated

