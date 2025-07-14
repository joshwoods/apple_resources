

- ML Compute
-  MLCReductionLayer Deprecated

Class

# MLCReductionLayer

A layer that reduces tensor values across a specific dimension to a scalar value.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCReductionLayer
```

## Overview

Use this layer to perform reduction operations on a given dimension. The output of this layer is a tensor of the same shape as the source tensor, except the layer sets the dimension to `1`.

## Topics

### Creating Reduction Layers

convenience init?(reductionType: MLCReductionType, dimension: Int)

Creates a reduction layer using the reduction type and dimension you specify.

convenience init?(reductionType: MLCReductionType, dimensions: [Int])

Creates a reduction layer using the reduction type and dimensions you specify.

enum MLCReductionType

Constants that describe a reduction operation type.

### Inspecting Reduction Layers

var reductionType: MLCReductionType

The function reduction type the system uses for reduction.

var dimension: Int

The dimension to perform the reduction operation on.

var dimensions: [Int]

The dimensions to perform the reduction operation on.

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

