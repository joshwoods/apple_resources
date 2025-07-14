

- Accelerate
- BNNSLayerParametersLSTM
-  init() Deprecated

Initializer

# init()

Returns a new long short-term memory (LSTM) parameters structure.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init()
```

Deprecated

Use BNNSGraph\* APIs

## Discussion

This initializer returns a new structure with all numeric properties set to `0`.

## See Also

### Initializers

init(input_size: Int, hidden_size: Int, batch_size: Int, num_layers: Int, seq_len: Int, dropout: Float, lstm_flags: UInt32, sequence_descriptor: BNNSNDArrayDescriptor, input_descriptor: BNNSLSTMDataDescriptor, output_descriptor: BNNSLSTMDataDescriptor, input_gate: BNNSLSTMGateDescriptor, forget_gate: BNNSLSTMGateDescriptor, candidate_gate: BNNSLSTMGateDescriptor, output_gate: BNNSLSTMGateDescriptor, hidden_activation: BNNSActivation)

Returns a new long short-term memory (LSTM) parameters structure from the specified parameters.

Deprecated

