

- ML Compute
- MLCOptimizerDescriptor
-  appliesGradientClipping Deprecated

Instance Property

# appliesGradientClipping

A Boolean that indicates whether you apply gradient clipping.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var appliesGradientClipping: Bool { get }
```

## Discussion

The default value is `false`.

## See Also

### Inspecting an Optimizer Descriptor

var learningRate: Float

The learning rate.

Deprecated

var gradientRescale: Float

The rescale value the optimizer applies to gradients during updates.

Deprecated

var gradientClipMax: Float

The maximum gradient value before the optimizer rescales the gradient, if you enabled gradient clipping.

Deprecated

var gradientClipMin: Float

The minimum gradient value before the optimizer rescales the gradient, if you enabled gradient clipping.

Deprecated

var regularizationScale: Float

The regularization scale.

Deprecated

var regularizationType: MLCRegularizationType

The regularization type.

Deprecated

var gradientClippingType: MLCGradientClippingType

The type of clipping the system applies to the gradient.

Deprecated

enum MLCGradientClippingType

A clipping type the system applies to a gradient.

Deprecated

var maximumClippingNorm: Float

The maximum clipping value.

Deprecated

var customGlobalNorm: Float

A custom norm the system uses in place of the global norm.

Deprecated

