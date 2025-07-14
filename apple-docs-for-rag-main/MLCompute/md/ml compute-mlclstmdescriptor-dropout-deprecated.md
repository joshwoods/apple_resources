

- ML Compute
- MLCLSTMDescriptor
-  dropout Deprecated

Instance Property

# dropout

The dropout probability.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var dropout: Float { get }
```

## Discussion

If `dropout` is non-zero, the layer adds a dropout layer to the outputs of each layer except the last, with the dropout rate equal to `dropout`.

## See Also

### Inspecting LSTM Descriptors

var batchFirst: Bool

A Boolean that indicates whether the input and output shape is batch first.

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

