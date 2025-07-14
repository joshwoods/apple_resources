

- Accelerate
- BNNSOptimizerAdamFields
-  learning_rate Deprecated

Instance Property

# learning_rate

A value that specifies the learning rate.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
var learning_rate: Float
```

Deprecated

Use BNNSGraph\* APIs

## See Also

### Instance Properties

var beta1: Float

A value that specifies the first moment constant in the range 0 to 1.

Deprecated

var beta2: Float

A value that specifies the second moment constant in the range 0 to 1.

Deprecated

var time_step: Float

A value that represents the optimizer’s current time and you’re responsible for updating after optimizing all the layer parameters in your network.

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

var clip_gradients: Bool

A Boolean value that specifies whether to clip the gradient between minimum and maximum values.

Deprecated

var clip_gradients_min: Float

The values for the minimum gradient.

Deprecated

var clip_gradients_max: Float

The values for the maximum gradient.

Deprecated

var regularization_func: BNNSOptimizerRegularizationFunction

The variable that specifies the regularization function.

Deprecated

