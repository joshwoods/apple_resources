

- ML Compute
- MLCTensor
-  init(shape:fillWithData:dataType:) Deprecated

Initializer

# init(shape:fillWithData:dataType:)

Creates a tensor with the shape, scalar value, and data type you specify.

iOS 14.0–17.0DeprecatediPadOS 14.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 11.0–14.0DeprecatedtvOS 14.0–17.0Deprecated

``` source
convenience init(
    shape: [Int],
    fillWithData fillData: NSNumber,
    dataType: MLCDataType
)
```

Deprecated

Use Metal Performance Shaders Graph or BNNS instead.

## Parameters 

`shape`  

An array that contains the sizes of each dimension.

`fillData`  

The scalar value with which to initialize the tensor data.

`dataType`  

The tensor data type.

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

convenience init(width: Int, height: Int, featureChannelCount: Int, batchSize: Int, randomInitializerType: MLCRandomInitializerType)

Creates a tensor with the sizes, number of feature channels, and random data using the random initializer type you specify.

Deprecated

