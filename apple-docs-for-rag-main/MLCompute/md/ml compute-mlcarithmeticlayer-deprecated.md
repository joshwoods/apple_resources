

- ML Compute
-  MLCArithmeticLayer Deprecated

Class

# MLCArithmeticLayer

A layer that performs an arithmetic operation.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCArithmeticLayer
```

## Topics

### Creating Arithmetic Layers

convenience init(operation: MLCArithmeticOperation)

Creates an arithmetic layer with the operation you specify.

enum MLCArithmeticOperation

Constants that describe an arithmetic operation.

### Inspecting Arithmetic Layers

var operation: MLCArithmeticOperation

The arithmetic layer’s operation.

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

### Math Layers

class MLCReductionLayer

A layer that reduces tensor values across a specific dimension to a scalar value.

Deprecated

class MLCMatMulLayer

A layer that multiplies matrices.

Deprecated

class MLCFullyConnectedLayer

A layer that connects each input to each output within its layer.

Deprecated

class MLCGramMatrixLayer

A layer that computes the uncentered cross-correlation values between the spacial planes of each feature channel of a tensor.

Deprecated

class MLCComparisonLayer

A layer that performs elementwise comparison of two tensors.

Deprecated

