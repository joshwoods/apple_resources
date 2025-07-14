

- ML Compute
-  MLCSoftmaxLayer Deprecated

Class

# MLCSoftmaxLayer

A layer that outputs a probability distribution as attention weights.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCSoftmaxLayer
```

## Topics

### Creating Softmax Layers

convenience init(operation: MLCSoftmaxOperation)

Creates a softmax layer with the operation you specify.

convenience init(operation: MLCSoftmaxOperation, dimension: Int)

Creates a softmax layer with the operation and dimension you specify.

enum MLCSoftmaxOperation

A softmax operation.

### Inspecting Softmax Layers

var operation: MLCSoftmaxOperation

The softmax operation.

var dimension: Int

The dimension over which you want to perform the softmax operation.

## Relationships

### Inherits From

- MLCLayer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Activation Layers

class MLCActivationLayer

A layer that applies an activation function to the source tensor and produces an output.

Deprecated

class MLCMultiheadAttentionLayer

A multihead, scaled dot-product attention layer that attends to one or more entries in the input key-value pairs.

Deprecated

