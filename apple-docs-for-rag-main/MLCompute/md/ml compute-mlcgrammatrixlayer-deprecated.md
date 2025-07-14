

- ML Compute
-  MLCGramMatrixLayer Deprecated

Class

# MLCGramMatrixLayer

A layer that computes the uncentered cross-correlation values between the spacial planes of each feature channel of a tensor.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCGramMatrixLayer
```

## Overview

For example, if the input tensor batch function is:

`x = x[b, y, x, c]`

The computation performed by this layer is:

`y = y[b, 1, f, c] = alpha * sum_{x, y} x[b, y, x, f] * x[b, y, x, c]`

Interpret this operation as computing all combinations of fully connected layers between the different spatial planes of the input tensor.

The layer performs this operation independently for each tensor in a batch. Then the layer stores these results in the feature channel and x-coordinate indices of the output batch.

Legend:

`b`  
The batch index.

`y` and `x`  
The spatial coordinates.

`c`  
The feature channel index.

`alpha`  
The scaling factor.

## Topics

### Creating Gram Matrix Layers

convenience init(scale: Float)

Creates a gram matrix layer with the scaling factor you specify.

### Inspecting Gram Matrix Layers

var scale: Float

The scaling factor.

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

class MLCComparisonLayer

A layer that performs elementwise comparison of two tensors.

Deprecated

