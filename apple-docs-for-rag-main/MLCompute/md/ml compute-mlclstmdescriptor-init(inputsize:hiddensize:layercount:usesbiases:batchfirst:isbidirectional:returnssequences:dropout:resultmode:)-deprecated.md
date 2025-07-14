

- ML Compute
- MLCLSTMDescriptor
-  init(inputSize:hiddenSize:layerCount:usesBiases:batchFirst:isBidirectional:returnsSequences:dropout:resultMode:) Deprecated

Initializer

# init(inputSize:hiddenSize:layerCount:usesBiases:batchFirst:isBidirectional:returnsSequences:dropout:resultMode:)

Creates a descriptor with the number of features and layers, dropout, and options for use of biases, batch order, return sequences, bidirectionality, and expected tensors you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init(
    inputSize: Int,
    hiddenSize: Int,
    layerCount: Int,
    usesBiases: Bool,
    batchFirst: Bool,
    isBidirectional: Bool,
    returnsSequences: Bool,
    dropout: Float,
    resultMode: MLCLSTMResultMode
)
```

## Parameters 

`inputSize`  

The number of expected features in the input.

`hiddenSize`  

The number of features in the hidden state.

`layerCount`  

The number of recurrent layers.

`usesBiases`  

A Boolean that indicates whether you use bias weights. The default value is `true`.

`batchFirst`  

A Boolean that indicates whether the first index of the input and output shape contains the batch size. The default value is `true`.

`isBidirectional`  

A Boolean that indicates whether the layer becomes bidirectional. The default value is `false`.

`returnsSequences`  

A Boolean that indicates whether the layer returns output for all sequences, or if `false`, returns output for only the last sequences. The default value is `true`.

`dropout`  

The dropout probability rate.

`resultMode`  

The expected result mode for the layer. The default value is MLCLSTMResultMode.output.

## See Also

### Creating LSTM Descriptors

convenience init(inputSize: Int, hiddenSize: Int, layerCount: Int)

Creates a batch first LSTM descriptor with the input size and number of layers you specify.

Deprecated

convenience init(inputSize: Int, hiddenSize: Int, layerCount: Int, usesBiases: Bool, isBidirectional: Bool, dropout: Float)

Creates a batch first LSTM descriptor with bias and bidirectional options you specify.

Deprecated

convenience init(inputSize: Int, hiddenSize: Int, layerCount: Int, usesBiases: Bool, batchFirst: Bool, isBidirectional: Bool, dropout: Float)

Creates a batch first LSTM descriptor that allows you to indicate whether the input and output shape is batch first.

Deprecated

convenience init(inputSize: Int, hiddenSize: Int, layerCount: Int, usesBiases: Bool, batchFirst: Bool, isBidirectional: Bool, returnsSequences: Bool, dropout: Float)

Creates a batch first LSTM descriptor that allows you to indicate whether the layer returns output for all sequences, or output for only the last sequence.

Deprecated

