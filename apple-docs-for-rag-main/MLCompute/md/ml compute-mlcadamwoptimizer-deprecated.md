

- ML Compute
-  MLCAdamWOptimizer Deprecated

Class

# MLCAdamWOptimizer

An optimizer that represents the Adam algorithm with weight decay.

iOS 15.0–17.4DeprecatediPadOS 15.0–17.4DeprecatedMac Catalyst 15.0–17.4DeprecatedmacOS 12.0–14.3DeprecatedtvOS 15.0–17.4Deprecated

``` source
class MLCAdamWOptimizer
```

## Topics

### Creating an AdamW Optimizer

convenience init(descriptor: MLCOptimizerDescriptor)

Creates a default optimizer with the descriptor you specify.

convenience init(descriptor: MLCOptimizerDescriptor, beta1: Float, beta2: Float, epsilon: Float, usesAMSGrad: Bool, timeStep: Int)

Creates an AdamW optimizer with the values you specify.

### Inspecting an AdamW Optimizer

var beta1: Float

The coefficent for computing running averages of gradient.

var beta2: Float

The coefficent for computing running averages of square of gradient.

var epsilon: Float

The epsilon value for improving numerical stability.

var timeStep: Int

The initial timestep for the update.

var usesAMSGrad: Bool

A Boolean value that indicates whether to use a variant of the algorithm.

## Relationships

### Inherits From

- MLCOptimizer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Optimizer Types

class MLCSGDOptimizer

An optimizer that represents the stochastic gradient decent algorithm.

Deprecated

class MLCRMSPropOptimizer

An optimizer that represents the root mean square propagation algorithm.

class MLCAdamOptimizer

An optimizer that represents the adaptive moment estimation algorithm.

Deprecated

class MLCOptimizer

The base class for all framework optimizers.

Deprecated

