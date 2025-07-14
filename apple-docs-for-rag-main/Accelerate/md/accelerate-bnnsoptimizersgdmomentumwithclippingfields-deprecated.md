

- Accelerate
-  BNNSOptimizerSGDMomentumWithClippingFields Deprecated

Structure

# BNNSOptimizerSGDMomentumWithClippingFields

A structure that contains the fields of a stochastic gradient descent (SGD) with momentum optimizer that optionally clips the gradient by value or by norm.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
struct BNNSOptimizerSGDMomentumWithClippingFields
```

Deprecated

Use BNNSGraph\* APIs

## Topics

### Initializers

init(learning_rate: Float, momentum: Float, gradient_scale: Float, regularization_scale: Float, nesterov: Bool, regularization_func: BNNSOptimizerRegularizationFunction, sgd_momentum_variant: BNNSOptimizerSGDMomentumVariant, clipping_func: BNNSOptimizerClippingFunction, clip_gradients_min: Float, clip_gradients_max: Float, clip_gradients_max_norm: Float, clip_gradients_use_norm: Float)

Returns a new SGD with momentum optimizer fields structure from the specified parameters.

init()

Returns a new SGD with momentum optimizer fields structure.

### Instance Properties

var learning_rate: Float

A value that specifies the learning rate.

var momentum: Float

The rate of momentum decay.

var gradient_scale: Float

A value that specifies the gradient scaling factor.

var regularization_scale: Float

A value that specifies the regularization scaling factor.

var nesterov: Bool

A Boolean value that specifies whether to use Nesterov momentum update.

var regularization_func: BNNSOptimizerRegularizationFunction

The variable that specifies the regularization function.

var sgd_momentum_variant: BNNSOptimizerSGDMomentumVariant

The variable that specifies the momentum variant.

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

struct BNNSOptimizerAdamWithClippingFields

A structure that contains the fields of an Adam or AdamW optimizer that optionally clips the gradient by value or by norm.

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

struct BNNSOptimizerSGDMomentumVariant

Constants that define SGD momentum variants.

func BNNSOptimizerStep(BNNSOptimizerFunction, UnsafeRawPointer, Int, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>>, UnsafeMutablePointer&lt;UnsafePointer&lt;BNNSNDArrayDescriptor>>, UnsafeMutablePointer&lt;UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?>?, UnsafePointer&lt;BNNSFilterParameters>?) -> Int32

Applies a single optimization step to one or more parameters.

Deprecated

struct BNNSOptimizerFunction

A structure that contains optimizer functions.

