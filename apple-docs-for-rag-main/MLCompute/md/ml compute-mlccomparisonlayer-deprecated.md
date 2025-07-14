

- ML Compute
-  MLCComparisonLayer Deprecated

Class

# MLCComparisonLayer

A layer that performs elementwise comparison of two tensors.

iOS 14.5–17.4DeprecatediPadOS 14.5–17.4DeprecatedMac Catalyst 14.5–17.4DeprecatedmacOS 11.3–14.3DeprecatedtvOS 14.5–17.4Deprecated

``` source
class MLCComparisonLayer
```

## Overview

The layer returns a tensor with the shape equal to the largest shape of operations. It fills with the Boolean value `result[i] = op1[i] ? op2[i]`, where `?` corresponds to the MLCComparisonOperation you specify.

## Topics

### Creating Comparison Layers

convenience init(operation: MLCComparisonOperation)

Creates a comparison layer with the operation you specify.

enum MLCComparisonOperation

A comparison operation.

### Inspecting Comparison Layers

var operation: MLCComparisonOperation

The comparison layer’s operation.

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

class MLCMatMulLayer

A layer that multiplies matrices.

Deprecated

class MLCFullyConnectedLayer

A layer that connects each input to each output within its layer.

Deprecated

class MLCGramMatrixLayer

A layer that computes the uncentered cross-correlation values between the spacial planes of each feature channel of a tensor.

Deprecated

