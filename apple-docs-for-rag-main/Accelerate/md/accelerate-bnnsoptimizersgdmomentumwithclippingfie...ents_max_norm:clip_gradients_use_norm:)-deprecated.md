

- Accelerate
- BNNSOptimizerSGDMomentumWithClippingFields
-  init(learning_rate:momentum:gradient_scale:regularization_scale:nesterov:regularization_func:sgd_momentum_variant:clipping_func:clip_gradients_min:clip_gradients_max:clip_gradients_max_norm:clip_gradients_use_norm:) Deprecated

Initializer

# init(learning_rate:momentum:gradient_scale:regularization_scale:nesterov:regularization_func:sgd_momentum_variant:clipping_func:clip_gradients_min:clip_gradients_max:clip_gradients_max_norm:clip_gradients_use_norm:)

Returns a new SGD with momentum optimizer fields structure from the specified parameters.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init(
    learning_rate: Float,
    momentum: Float,
    gradient_scale: Float,
    regularization_scale: Float,
    nesterov: Bool,
    regularization_func: BNNSOptimizerRegularizationFunction,
    sgd_momentum_variant: BNNSOptimizerSGDMomentumVariant,
    clipping_func: BNNSOptimizerClippingFunction,
    clip_gradients_min: Float,
    clip_gradients_max: Float,
    clip_gradients_max_norm: Float,
    clip_gradients_use_norm: Float
)
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`learning_rate`  

A value that specifies the learning rate.

`momentum`  

The rate of momentum decay.

`gradient_scale`  

A value that specifies the gradient scaling factor.

`regularization_scale`  

A value that specifies the regularization scaling factor.

`nesterov`  

A Boolean value that specifies whether to use Nesterov momentum update.

`regularization_func`  

The variable that specifies the regularization function.

`sgd_momentum_variant`  

The variable that specifies the momentum variant.

`clipping_func`  

The clipping function.

`clip_gradients_min`  

The minimum clipping value for clipping by value.

`clip_gradients_max`  

The maximum clipping value for clipping by value.

`clip_gradients_max_norm`  

The maximum Euclidean norm for clipping by norm and clipping by global norm.

`clip_gradients_use_norm`  

An optional value for a known Euclidean norm for clipping by global norm. Set to `0` to specify that the function computes the norm.

## See Also

### Related Documentation

struct BNNSOptimizerClippingFunction

Constants that describe clipping functions.

### Initializers

init()

Returns a new SGD with momentum optimizer fields structure.

Deprecated

