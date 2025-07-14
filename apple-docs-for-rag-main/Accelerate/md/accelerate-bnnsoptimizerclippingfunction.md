

- Accelerate
-  BNNSOptimizerClippingFunction 

Structure

# BNNSOptimizerClippingFunction

Constants that describe clipping functions.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct BNNSOptimizerClippingFunction
```

## Topics

### Clipping Functions

init(UInt32)

Creates a new instance with the specified raw value.

init(rawValue: UInt32)

Creates a new instance with the specified raw value.

var rawValue: UInt32

The corresponding value of the raw type.

var BNNSOptimizerClippingNone: BNNSOptimizerClippingFunction

A constant that specifes no clipping.

var BNNSOptimizerClippingByValue: BNNSOptimizerClippingFunction

A constant that specifes clipping to minimum and maximum values.

var BNNSOptimizerClippingByNorm: BNNSOptimizerClippingFunction

A constant that specifes clipping to a maximum Euclidean norm.

var BNNSOptimizerClippingByGlobalNorm: BNNSOptimizerClippingFunction

A constant that specifes clipping to a maximum global Euclidean norm.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Instance Properties

var learning_rate: Float

A value that specifies the learning rate.

Deprecated

var beta1: Float

A value that specifies the first moment constant in the range 0 to 1.

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

