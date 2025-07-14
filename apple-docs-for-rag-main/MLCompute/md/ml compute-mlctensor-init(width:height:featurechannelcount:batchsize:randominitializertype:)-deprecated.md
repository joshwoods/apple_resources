

- ML Compute
- MLCTensor
-  init(width:height:featureChannelCount:batchSize:randomInitializerType:) Deprecated

Initializer

# init(width:height:featureChannelCount:batchSize:randomInitializerType:)

Creates a tensor with the sizes, number of feature channels, and random data using the random initializer type you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init(
    width: Int,
    height: Int,
    featureChannelCount: Int,
    batchSize: Int,
    randomInitializerType: MLCRandomInitializerType
)
```

## Parameters 

`width`  

The tensor width.

`height`  

The tensor height.

`featureChannelCount`  

The number of feature channels.

`batchSize`  

The tensor batch size.

`randomInitializerType`  

The random initializer type you use to generate random data.

## See Also

### Creating Tensors by Specifying Shape

convenience init(shape: [Int])

Creates a tensor without data, with the shape you specify.

Deprecated

convenience init(shape: [Int], dataType: MLCDataType)

Creates a tensor without data, with the shape and data type you specify.

Deprecated

convenience init(shape: [Int], data: MLCTensorData, dataType: MLCDataType)

Creates a tensor with the shape, data, and data type you specify.

Deprecated

convenience init(shape: [Int], fillWithData: NSNumber, dataType: MLCDataType)

Creates a tensor with the shape, scalar value, and data type you specify.

Deprecated

convenience init(shape: [Int], randomInitializerType: MLCRandomInitializerType)

Creates a tensor with the shape and random initializer type you specify.

Deprecated

convenience init(width: Int, height: Int, featureChannelCount: Int, batchSize: Int)

Creates a tensor without data, with the sizes and number of feature channels you specify.

Deprecated

convenience init(width: Int, height: Int, featureChannelCount: Int, batchSize: Int, data: MLCTensorData)

Creates a tensor with the sizes, number of feature channels, and data you specify.

Deprecated

convenience init(width: Int, height: Int, featureChannelCount: Int, batchSize: Int, data: MLCTensorData, dataType: MLCDataType)

Creates a tensor with the sizes, number of feature channels, data, and data type you specify.

Deprecated

convenience init(width: Int, height: Int, featureChannelCount: Int, batchSize: Int, fillWithData: Float, dataType: MLCDataType)

Creates a tensor with the sizes and number of feature channels, and filled with the data and type you specify.

Deprecated

