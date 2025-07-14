

- Accelerate
- BNNSOptimizerRMSPropWithClippingFields
-  clipping_func Deprecated

Instance Property

# clipping_func

The clipping function.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
var clipping_func: BNNSOptimizerClippingFunction
```

Deprecated

Use BNNSGraph\* APIs

## See Also

### Instance Properties

var learning_rate: Float

A value that specifies the learning rate.

Deprecated

var alpha: Float

A constant that specifies smoothing.

Deprecated

var epsilon: Float

A term that the optimizer adds to the denominator.

Deprecated

var centered: Bool

A Boolean value that specifies whether to use the centered variant.

Deprecated

var momentum: Float

The rate of momentum decay.

Deprecated

var gradient_scale: Float

A value that specifies the gradient scaling factor.

Deprecated

var regularization_scale: Float

A value that specifies the regularization scaling factor.

Deprecated

var regularization_func: BNNSOptimizerRegularizationFunction

The variable that specifies the regularization function.

Deprecated

struct BNNSOptimizerClippingFunction

Constants that describe clipping functions.

var clip_gradients_min: Float

The minimum clipping value for clipping by value.

Deprecated

var clip_gradients_max: Float

The maximum clipping value for clipping by value.

Deprecated

var clip_gradients_max_norm: Float

The maximum Euclidean norm for clipping by norm and clipping by global norm.

Deprecated

var clip_gradients_use_norm: Float

An optional value for a known Euclidean norm for clipping by global norm.

Deprecated

