

- ML Compute
-  MLCOptimizer Deprecated

Class

# MLCOptimizer

The base class for all framework optimizers.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCOptimizer
```

## Topics

### Inspecting an Optimizer

var learningRate: Float

The learning rate.

var gradientRescale: Float

The rescale value the optimizer applies to gradients during updates.

var appliesGradientClipping: Bool

A Boolean value that indicates whether you apply gradient clipping.

var gradientClipMax: Float

The maximum gradient value before the optimizer rescales the gradient, if you enable gradient clipping.

var gradientClipMin: Float

The minimum gradient value before the optimizer rescales the gradient, if you enable gradient clipping.

var regularizationScale: Float

The regularization scale.

var regularizationType: MLCRegularizationType

The regularization type.

var gradientClippingType: MLCGradientClippingType

The type of clipping the system applies to the gradient.

enum MLCGradientClippingType

A clipping type the system applies to a gradient.

var maximumClippingNorm: Float

The maximum clipping value.

var customGlobalNorm: Float

A custom norm the system uses in place of the global norm.

## Relationships

### Inherits From

- NSObject

### Inherited By

- MLCAdamOptimizer
- MLCAdamWOptimizer
- MLCRMSPropOptimizer
- MLCSGDOptimizer

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

class MLCAdamWOptimizer

An optimizer that represents the Adam algorithm with weight decay.

Deprecated

