

- Accelerate
-  BNNSOptimizerAdamWithClippingFields Deprecated

Structure

# BNNSOptimizerAdamWithClippingFields

A structure that contains the fields of an Adam or AdamW optimizer that optionally clips the gradient by value or by norm.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
struct BNNSOptimizerAdamWithClippingFields
```

Deprecated

Use BNNSGraph\* APIs

## Topics

### Initializers

init(learning_rate: Float, beta1: Float, beta2: Float, time_step: Float, epsilon: Float, gradient_scale: Float, regularization_scale: Float, regularization_func: BNNSOptimizerRegularizationFunction, clipping_func: BNNSOptimizerClippingFunction, clip_gradients_min: Float, clip_gradients_max: Float, clip_gradients_max_norm: Float, clip_gradients_use_norm: Float)

Returns a new Adam or AdamW optimizer fields structure from the specified parameters.

init()

Returns a new Adam or AdamW optimizer fields structure.

### Instance Properties

var learning_rate: Float

A value that specifies the learning rate.

var beta1: Float

A value that specifies the first moment constant in the range 0 to 1.

var beta2: Float

A value that specifies the second moment constant in the range 0 to 1.

var time_step: Float

A value that’s at least 1 and represents the optimizer’s current time.

var epsilon: Float

An addition for the division in the parameter update stage.

var gradient_scale: Float

A value that specifies the gradient scaling factor.

var regularization_scale: Float

A value that specifies the regularization scaling factor.

var regularization_func: BNNSOptimizerRegularizationFunction

The variable that specifies the regularization function.

var clipping_func: BNNSOptimizerClippingFunction

The clipping function.

struct BNNSOptimizerClippingFunction

Constants that describe clipping functions.

var clip_gradients_min: Float

The minimum clipping value for clipping by value.

var clip_gradients_max: Float

The maximum clipping value for clipping by value.

var clip_gradients_max_norm: Float

The maximum Euclidean norm for clipping by norm and clipping by global norm.

var clip_gradients_use_norm: Float

An optional value for a known Euclidean norm for clipping by global norm.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Optimizers

struct AdamOptimizer

An optimizer that uses the Adam optimization algorithm.

Deprecated

struct AdamWOptimizer

An optimizer that uses the AdamW optimization algorithm.

Deprecated

struct RMSPropOptimizer

An optimizer that uses the root mean square propagation (RMSProp) optimization method.

Deprecated

struct SGDMomentumOptimizer

An optimizer that uses the stochastic gradient descent (SGD) with the momentum optimization method.

Deprecated

protocol BNNSOptimizerDeprecated

struct BNNSOptimizerRegularizationFunction

A structure that contains optimizer regularization functions.

struct BNNSOptimizerAdamFields

A structure that contains the fields of an Adam optimizer.

Deprecated

struct BNNSOptimizerRMSPropFields

A structure that contains the fields of a root mean square propagation (RMSProp) optimizer.

Deprecated

struct BNNSOptimizerRMSPropWithClippingFields

A structure that contains the fields of a root mean square propagation (RMSProp) optimizer that optionally clips the gradient by value or by norm.

Deprecated

struct BNNSOptimizerSGDMomentumFields

A structure that contains the fields of a stochastic gradient descent (SGD) with momentum optimizer.

Deprecated

struct BNNSOptimizerSGDMomentumWithClippingFields

A structure that contains the fields of a stochastic gradient descent (SGD) with momentum optimizer that optionally clips the gradient by value or by norm.

Deprecated

struct BNNSOptimizerSGDMomentumVariant

Constants that define SGD momentum variants.

func BNNSOptimizerStep(BNNSOptimizerFunction, UnsafeRawPointer, Int, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>>, UnsafeMutablePointer&lt;UnsafePointer&lt;BNNSNDArrayDescriptor>>, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?>?, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Applies a single optimization step to one or more parameters.

Deprecated

struct BNNSOptimizerFunction

A structure that contains optimizer functions.

