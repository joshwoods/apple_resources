

- ML Compute
-  MLCOptimizerDescriptor Deprecated

Class

# MLCOptimizerDescriptor

A configuration object you use to create an optimizer.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCOptimizerDescriptor
```

## Topics

### Creating an Optimizer Descriptor

convenience init(learningRate: Float, gradientRescale: Float, regularizationType: MLCRegularizationType, regularizationScale: Float)

Creates an optimizer descriptor with the learning rate, gradient rescale, regularization type, and regulation scale that you specify.

convenience init(learningRate: Float, gradientRescale: Float, appliesGradientClipping: Bool, gradientClipMax: Float, gradientClipMin: Float, regularizationType: MLCRegularizationType, regularizationScale: Float)

Creates a descriptor with the learning rate, gradient rescale, clipping option and values, and regularization type and scale that you specify.

convenience init(learningRate: Float, gradientRescale: Float, appliesGradientClipping: Bool, gradientClippingType: MLCGradientClippingType, gradientClipMax: Float, gradientClipMin: Float, maximumClippingNorm: Float, customGlobalNorm: Float, regularizationType: MLCRegularizationType, regularizationScale: Float)

Creates a descriptor with the learning rate, gradient rescale, clipping option and values, and regularization type and scale that you specify.

### Inspecting an Optimizer Descriptor

var learningRate: Float

The learning rate.

var gradientRescale: Float

The rescale value the optimizer applies to gradients during updates.

var appliesGradientClipping: Bool

A Boolean that indicates whether you apply gradient clipping.

var gradientClipMax: Float

The maximum gradient value before the optimizer rescales the gradient, if you enabled gradient clipping.

var gradientClipMin: Float

The minimum gradient value before the optimizer rescales the gradient, if you enabled gradient clipping.

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

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Supporting Types

enum MLCRegularizationType

A regularization function to use with an optimizer.

Deprecated

