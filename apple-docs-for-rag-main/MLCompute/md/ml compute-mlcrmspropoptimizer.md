

- ML Compute
-  MLCRMSPropOptimizer 

Class

# MLCRMSPropOptimizer

An optimizer that represents the root mean square propagation algorithm.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.2+macOS 11.0–15.4DeprecatedtvOS 14.0+

``` source
class MLCRMSPropOptimizer
```

## Topics

### Creating an RMSProp Optimizer

convenience init(descriptor: MLCOptimizerDescriptor)

Creates an RMSProp optimizer with the descriptor you specify.

convenience init(descriptor: MLCOptimizerDescriptor, momentumScale: Float, alpha: Float, epsilon: Float, isCentered: Bool)

Creates an RMSProp optimizer with the descriptor, momentum scale, smoothing, epsilon, and option to compute the centered RMSProp that you specify.

### Inspecting an RMSProp Optimizer

var momentumScale: Float

A hyper-parameter that specifies the momentum factor.

var alpha: Float

The constant for smoothing.

var epsilon: Float

The epsilon value you use to improve numerical stability.

var isCentered: Bool

A Boolean that indicates whether you compute the centered RMSProp.

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

class MLCAdamOptimizer

An optimizer that represents the adaptive moment estimation algorithm.

Deprecated

class MLCAdamWOptimizer

An optimizer that represents the Adam algorithm with weight decay.

Deprecated

class MLCOptimizer

The base class for all framework optimizers.

Deprecated

