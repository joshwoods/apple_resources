

- ML Compute
- MLCTensor
-  init(descriptor:) Deprecated

Initializer

# init(descriptor:)

Creates a tensor without data, using the descriptor you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init(descriptor tensorDescriptor: MLCTensorDescriptor)
```

## Parameters 

`tensorDescriptor`  

An object you use to configure the tensor.

## Discussion

The tensor data type is MLCDataType.float32.

## See Also

### Creating Tensors with Descriptors

convenience init(descriptor: MLCTensorDescriptor, data: MLCTensorData)

Creates a tensor with the descriptor and data you specify.

Deprecated

convenience init(descriptor: MLCTensorDescriptor, fillWithData: NSNumber)

Creates a tensor with the descriptor and scalar value you specify.

Deprecated

convenience init(descriptor: MLCTensorDescriptor, randomInitializerType: MLCRandomInitializerType)

Creates a tensor with the descriptor and random initializer type you specify.

Deprecated

class MLCTensorDescriptor

A configuration object you use to create a tensor.

Deprecated

enum MLCDataType

A tensor data type.

Deprecated

class MLCTensorData

An encapsulation of the memory that tensor data uses.

Deprecated

enum MLCRandomInitializerType

An initializer type you use to create a tensor with random data.

Deprecated

