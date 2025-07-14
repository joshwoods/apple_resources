

- Accelerate
- BNNSOptimizerAdamWithClippingFields
-  beta1 Deprecated

Instance Property

# beta1

A value that specifies the first moment constant in the range 0 to 1.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
var beta1: Float
```

Deprecated

Use BNNSGraph\* APIs

## See Also

### Instance Properties

var learning_rate: Float

A value that specifies the learning rate.

Deprecated

var beta2: Float

A value that specifies the second moment constant in the range 0 to 1.

Deprecated

var time_step: Float

A value that’s at least 1 and represents the optimizer’s current time.

Deprecated

var epsilon: Float

An addition for the division in the parameter update stage.

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

var clipping_func: BNNSOptimizerClippingFunction

The clipping function.

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

