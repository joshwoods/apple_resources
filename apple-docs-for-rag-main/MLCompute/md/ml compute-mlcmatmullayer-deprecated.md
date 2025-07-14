

- ML Compute
-  MLCMatMulLayer Deprecated

Class

# MLCMatMulLayer

A layer that multiplies matrices.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCMatMulLayer
```

## Topics

### Creating Matrix Multiplication Layers

convenience init?(descriptor: MLCMatMulDescriptor)

Creates a matrix multiplication layer with the specified descriptor you specify.

class MLCMatMulDescriptor

A configuration object you use to create a matrix multiplication layer.

### Inspecting Matrix Multiplication Layers

var descriptor: MLCMatMulDescriptor

The configuration object you use to create the matrix multiplication layer.

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

class MLCArithmeticLayer

A layer that performs an arithmetic operation.

Deprecated

class MLCReductionLayer

A layer that reduces tensor values across a specific dimension to a scalar value.

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

