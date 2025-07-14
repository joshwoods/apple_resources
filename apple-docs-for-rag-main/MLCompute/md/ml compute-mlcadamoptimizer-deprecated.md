

- ML Compute
-  MLCAdamOptimizer Deprecated

Class

# MLCAdamOptimizer

An optimizer that represents the adaptive moment estimation algorithm.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCAdamOptimizer
```

## Topics

### Creating an Adam Optimizer

convenience init(descriptor: MLCOptimizerDescriptor)

Creates an Adam optimizer with the descriptor you specify.

convenience init(descriptor: MLCOptimizerDescriptor, beta1: Float, beta2: Float, epsilon: Float, timeStep: Int)

Creates an Adam optimizer with the values you specify.

convenience init(descriptor: MLCOptimizerDescriptor, beta1: Float, beta2: Float, epsilon: Float, usesAMSGrad: Bool, timeStep: Int)

Creates an Adam optimizer with the values you specify.

### Inspecting an Adam Optimizer

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

class MLCAdamWOptimizer

An optimizer that represents the Adam algorithm with weight decay.

Deprecated

class MLCOptimizer

The base class for all framework optimizers.

Deprecated

