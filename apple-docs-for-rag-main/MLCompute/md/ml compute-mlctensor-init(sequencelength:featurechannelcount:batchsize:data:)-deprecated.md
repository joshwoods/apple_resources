

- ML Compute
- MLCTensor
-  init(sequenceLength:featureChannelCount:batchSize:data:) Deprecated

Initializer

# init(sequenceLength:featureChannelCount:batchSize:data:)

Creates a tensor with the sequence length, number of feature channels, batch size, and data you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init(
    sequenceLength: Int,
    featureChannelCount: Int,
    batchSize: Int,
    data: MLCTensorData?
)
```

## Parameters 

`sequenceLength`  

The length of sequences stored in the tensor.

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

convenience init?(sequenceLengths: [Int], sortedSequences: Bool, featureChannelCount: Int, batchSize: Int, data: MLCTensorData?)

Creates a tensor with the sequence lengths, sorting indicator, number of feature channels, batch size, and data you specify.

Deprecated

convenience init(sequenceLength: Int, featureChannelCount: Int, batchSize: Int, randomInitializerType: MLCRandomInitializerType)

Creates a tensor with the sequence length, number of feature channels, batch size, and random initializer type you specify.

Deprecated

convenience init?(sequenceLengths: [Int], sortedSequences: Bool, featureChannelCount: Int, batchSize: Int, randomInitializerType: MLCRandomInitializerType)

Creates a tensor with the sequence lengths, sorting indicator, number of feature channels, batch size, and random initializer type you specify.

Deprecated

