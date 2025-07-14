

- ML Compute
- MLCLSTMDescriptor
-  init(inputSize:hiddenSize:layerCount:) Deprecated

Initializer

# init(inputSize:hiddenSize:layerCount:)

Creates a batch first LSTM descriptor with the input size and number of layers you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init(
    inputSize: Int,
    hiddenSize: Int,
    layerCount: Int
)
```

## Parameters 

`inputSize`  

The number of expected features in the input.

`hiddenSize`  

The number of features in the hidden state.

`layerCount`  

The number of recurrent layers.

## See Also

### Creating LSTM Descriptors

convenience init(inputSize: Int, hiddenSize: Int, layerCount: Int, usesBiases: Bool, isBidirectional: Bool, dropout: Float)

Creates a batch first LSTM descriptor with bias and bidirectional options you specify.

Deprecated

convenience init(inputSize: Int, hiddenSize: Int, layerCount: Int, usesBiases: Bool, batchFirst: Bool, isBidirectional: Bool, dropout: Float)

Creates a batch first LSTM descriptor that allows you to indicate whether the input and output shape is batch first.

Deprecated

convenience init(inputSize: Int, hiddenSize: Int, layerCount: Int, usesBiases: Bool, batchFirst: Bool, isBidirectional: Bool, returnsSequences: Bool, dropout: Float)

Creates a batch first LSTM descriptor that allows you to indicate whether the layer returns output for all sequences, or output for only the last sequence.

Deprecated

convenience init(inputSize: Int, hiddenSize: Int, layerCount: Int, usesBiases: Bool, batchFirst: Bool, isBidirectional: Bool, returnsSequences: Bool, dropout: Float, resultMode: MLCLSTMResultMode)

Creates a descriptor with the number of features and layers, dropout, and options for use of biases, batch order, return sequences, bidirectionality, and expected tensors you specify.

Deprecated

