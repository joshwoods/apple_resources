

- ML Compute
- MLCTensor
-  init(sequenceLengths:sortedSequences:featureChannelCount:batchSize:data:) Deprecated

Initializer

# init(sequenceLengths:sortedSequences:featureChannelCount:batchSize:data:)

Creates a tensor with the sequence lengths, sorting indicator, number of feature channels, batch size, and data you specify.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
convenience init?(
    sequenceLengths: [Int],
    sortedSequences: Bool,
    featureChannelCount: Int,
    batchSize: Int,
    data: MLCTensorData? = nil
)
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## Parameters 

`sequenceLengths`  

An array that contains the variable lengths of sequences stored in the tensor.

`sortedSequences`  

A Boolean that indicates whether you provide the sequence lengths sorted in descending order.

`featureChannelCount`  

The number of feature channels.

`batchSize`  

The tensor batch size.

`data`  

The tensor data.

## See Also

### Creating Tensors by Specifying Sequence Lengths

convenience init(sequenceLength: Int, featureChannelCount: Int, batchSize: Int)

Creates a tensor without data, with the sequence length, number of feature channels, and batch size you specify.

Deprecated

convenience init(sequenceLength: Int, featureChannelCount: Int, batchSize: Int, data: MLCTensorData?)

Creates a tensor with the sequence length, number of feature channels, batch size, and data you specify.

Deprecated

convenience init(sequenceLength: Int, featureChannelCount: Int, batchSize: Int, randomInitializerType: MLCRandomInitializerType)

Creates a tensor with the sequence length, number of feature channels, batch size, and random initializer type you specify.

Deprecated

convenience init?(sequenceLengths: [Int], sortedSequences: Bool, featureChannelCount: Int, batchSize: Int, randomInitializerType: MLCRandomInitializerType)

Creates a tensor with the sequence lengths, sorting indicator, number of feature channels, batch size, and random initializer type you specify.

Deprecated

