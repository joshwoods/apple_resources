

- ML Compute
-  MLCSGDOptimizer Deprecated

Class

# MLCSGDOptimizer

An optimizer that represents the stochastic gradient decent algorithm.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCSGDOptimizer
```

## Topics

### Creating an SGD Optimizer

convenience init(descriptor: MLCOptimizerDescriptor)

Creates an SGD optimizer with the descriptor you specify.

convenience init(descriptor: MLCOptimizerDescriptor, momentumScale: Float, usesNesterovMomentum: Bool)

Create an SGD optimizer with the descriptor, momentum scale, and option to enable Nesterov momentum that you specify.

### Inspecting an SGD Optimizer

var momentumScale: Float

A hyper-parameter specifying the momentum factor.

var usesNesterovMomentum: Bool

A Boolean that indicates whether you enable Nesterov momentum.

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

class MLCRMSPropOptimizer

An optimizer that represents the root mean square propagation algorithm.

class MLCAdamOptimizer

An optimizer that represents the adaptive moment estimation algorithm.

Deprecated

class MLCAdamWOptimizer

An optimizer that represents the Adam algorithm with weight decay.

Deprecated

class MLCOptimizer

The base class for all framework optimizers.

Deprecated

