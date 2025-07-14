

- ML Compute
- MLCTensorDescriptor
-  init(width:height:featureChannelCount:batchSize:) Deprecated

Initializer

# init(width:height:featureChannelCount:batchSize:)

Creates a tensor descriptor with the width and height, number of feature channels, and batch size you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init?(
    width: Int,
    height: Int,
    featureChannelCount featureChannels: Int,
    batchSize: Int
)
```

## Parameters 

`width`  

The tensor width.

`height`  

The tensor height.

`featureChannels`  

The number of feature channels.

`batchSize`  

The tensor batch size.

## Discussion

This initializer provides a convenient way for you to configure NCHW tensors used by convolutional layers. The tensor data type is MLCDataType.float32.

## See Also

### Creating Tensor Descriptors

convenience init?(shape: [Int], dataType: MLCDataType)

Creates a tensor descriptor with the shape and data type you specify.

Deprecated

convenience init?(shape: [Int], sequenceLengths: [Int], sortedSequences: Bool, dataType: MLCDataType)

Creates a tensor descriptor with the shape, variable sequence lengths, sorting indicator, and data type you specify.

Deprecated

convenience init?(width: Int, height: Int, featureChannelCount: Int, batchSize: Int, dataType: MLCDataType)

Creates a tensor descriptor with the width and height, number of feature channels, batch size, and data type you specify.

Deprecated

convenience init?(convolutionWeightsWithInputFeatureChannelCount: Int, outputFeatureChannelCount: Int, dataType: MLCDataType)

Creates a tensor descriptor with the number of feature channels and data type you specify.

Deprecated

convenience init?(convolutionWeightsWithWidth: Int, height: Int, inputFeatureChannelCount: Int, outputFeatureChannelCount: Int, dataType: MLCDataType)

Creates a tensor descriptor with the sizing, number of feature channels, and data type you specify.

Deprecated

convenience init?(convolutionBiasesWithFeatureChannelCount: Int, dataType: MLCDataType)

Creates a tensor descriptor with the number of feature channels and data type you specify.

Deprecated

class var maxTensorDimensions: Int

The maximum number of tensor dimensions.

Deprecated

