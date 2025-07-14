

- ML Compute
-  MLCRandomInitializerType Deprecated

Enumeration

# MLCRandomInitializerType

An initializer type you use to create a tensor with random data.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
enum MLCRandomInitializerType
```

## Topics

### Enumeration Cases

case uniform

case glorotUniform

case xavier

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating Tensors with Descriptors

convenience init(descriptor: MLCTensorDescriptor)

Creates a tensor without data, using the descriptor you specify.

Deprecated

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

