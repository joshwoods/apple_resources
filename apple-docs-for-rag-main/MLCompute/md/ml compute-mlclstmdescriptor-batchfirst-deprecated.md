

- ML Compute
- MLCLSTMDescriptor
-  batchFirst Deprecated

Instance Property

# batchFirst

A Boolean that indicates whether the input and output shape is batch first.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var batchFirst: Bool { get }
```

## Discussion

If `batchFirst` is `true`, the input and output shape is `[batch, feature, 1, time steps]`. Otherwise, the shape is `[time steps, batch, feature]`, which is more efficient.

## See Also

### Inspecting LSTM Descriptors

var dropout: Float

The dropout probability.

Deprecated

var hiddenSize: Int

The number of features in the hidden state.

Deprecated

var inputSize: Int

The number of expected features in the input.

Deprecated

var isBidirectional: Bool

A Boolean that indicates whether the layer is bidirectional.

Deprecated

var layerCount: Int

The number of recurrent layers.

Deprecated

var resultMode: MLCLSTMResultMode

The mode that indicates whether the layer produces a single result tensor or three result tensors — final output, last hidden state, and the cell state.

Deprecated

var returnsSequences: Bool

A Boolean that indicates whether the layer returns output for all sequences.

Deprecated

var usesBiases: Bool

A Boolean that indicates whether you use bias weights.

Deprecated

