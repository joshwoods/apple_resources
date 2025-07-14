

- Accelerate
- BNNSLSTMGateDescriptor
-  cw_desc Deprecated

Instance Property

# cw_desc

The descriptor of the cell weights.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
var cw_desc: BNNSNDArrayDescriptor
```

Deprecated

Use BNNSGraph\* APIs

## Discussion

Weights are ordered as `[num_layers][num_directions][hidden_size][hidden_size]` (C style multi array notation).

## See Also

### Instance Properties

var iw_desc: (BNNSNDArrayDescriptor, BNNSNDArrayDescriptor)

The descriptor of the input weights.

Deprecated

var hw_desc: BNNSNDArrayDescriptor

The descriptor of the hidden weights.

Deprecated

var b_desc: BNNSNDArrayDescriptor

The descriptor of the bias.

Deprecated

var activation: BNNSActivation

The activation function that the layer applies to the output.

Deprecated

