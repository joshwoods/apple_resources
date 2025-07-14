

- ML Compute
-  MLCSoftmaxOperation Deprecated

Enumeration

# MLCSoftmaxOperation

A softmax operation.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
enum MLCSoftmaxOperation
```

## Topics

### Enumeration Cases

case softmax

case logSoftmax

var debugDescription: String

A textual description of the softmax operation, suitable for debugging.

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

### Creating Softmax Layers

convenience init(operation: MLCSoftmaxOperation)

Creates a softmax layer with the operation you specify.

Deprecated

convenience init(operation: MLCSoftmaxOperation, dimension: Int)

Creates a softmax layer with the operation and dimension you specify.

Deprecated

