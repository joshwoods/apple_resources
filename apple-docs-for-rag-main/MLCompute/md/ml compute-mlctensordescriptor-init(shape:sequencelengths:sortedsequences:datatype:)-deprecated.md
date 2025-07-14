

- ML Compute
- MLCTensorDescriptor
-  init(shape:sequenceLengths:sortedSequences:dataType:) Deprecated

Initializer

# init(shape:sequenceLengths:sortedSequences:dataType:)

Creates a tensor descriptor with the shape, variable sequence lengths, sorting indicator, and data type you specify.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
convenience init?(
    shape: [Int],
    sequenceLengths: [Int],
    sortedSequences: Bool,
    dataType: MLCDataType
)
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## Parameters 

`shape`  

The tensor shape.

`sequenceLengths`  

An array of the variable length of sequences stored in the tensor.

`sortedSequences`  

A Boolean that indicates whether you provide the sequence lengths sorted in descending order.

`dataType`  

The tensor data type.

## Discussion

This initializer provides a convenient way for you to configure sequence tensors used by recurrent layers.

## See Also

### Creating Tensor Descriptors

convenience init?(shape: [Int], dataType: MLCDataType)

Creates a tensor descriptor with the shape and data type you specify.

Deprecated

convenience init?(width: Int, height: Int, featureChannelCount: Int, batchSize: Int)

Creates a tensor descriptor with the width and height, number of feature channels, and batch size you specify.

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

