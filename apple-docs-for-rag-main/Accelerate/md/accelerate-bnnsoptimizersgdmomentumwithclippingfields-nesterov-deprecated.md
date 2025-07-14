

- Accelerate
- BNNSOptimizerSGDMomentumWithClippingFields
-  nesterov Deprecated

Instance Property

# nesterov

A Boolean value that specifies whether to use Nesterov momentum update.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
var nesterov: Bool
```

Deprecated

Use BNNSGraph\* APIs

## See Also

### Instance Properties

var learning_rate: Float

A value that specifies the learning rate.

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

var sgd_momentum_variant: BNNSOptimizerSGDMomentumVariant

The variable that specifies the momentum variant.

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

