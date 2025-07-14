

- Accelerate
- BNNSOptimizerRMSPropFields
-  init(learning_rate:alpha:epsilon:centered:momentum:gradient_scale:regularization_scale:clip_gradients:clip_gradients_min:clip_gradients_max:regularization_func:) Deprecated

Initializer

# init(learning_rate:alpha:epsilon:centered:momentum:gradient_scale:regularization_scale:clip_gradients:clip_gradients_min:clip_gradients_max:regularization_func:)

Returns a new RMSProp optimizer fields structure from the specified parameters.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init(
    learning_rate: Float,
    alpha: Float,
    epsilon: Float,
    centered: Bool,
    momentum: Float,
    gradient_scale: Float,
    regularization_scale: Float,
    clip_gradients: Bool,
    clip_gradients_min: Float,
    clip_gradients_max: Float,
    regularization_func: BNNSOptimizerRegularizationFunction
)
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`learning_rate`  

A value that specifies the learning rate.

`alpha`  

A constant that specifies smoothing, in the range 0 to 1.

`epsilon`  

A term that the optimizer adds to the denominator.

`centered`  

A Boolean value that specifies whether to use the centered variant.

`momentum`  

The rate of momentum decay.

`gradient_scale`  

A value that specifies the gradient scaling factor.

`regularization_scale`  

A value that specifies the regularization scaling factor.

`clip_gradients`  

A Boolean value that specifies whether to clip the gradient between minimum and maximum values.

`clip_gradients_min`  

The values for the minimum gradient.

`clip_gradients_max`  

The values for the maximum gradient.

`regularization_func`  

The variable that specifies the regularization function.

## See Also

### Initializers

init()

Returns a new RMSProp optimizer fields structure.

Deprecated

