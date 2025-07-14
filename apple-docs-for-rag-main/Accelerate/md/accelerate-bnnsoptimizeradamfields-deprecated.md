

- Accelerate
-  BNNSOptimizerAdamFields Deprecated

Structure

# BNNSOptimizerAdamFields

A structure that contains the fields of an Adam optimizer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
struct BNNSOptimizerAdamFields
```

Deprecated

Use BNNSGraph\* APIs

## Topics

### Initializers

init(learning_rate: Float, beta1: Float, beta2: Float, time_step: Float, epsilon: Float, gradient_scale: Float, regularization_scale: Float, clip_gradients: Bool, clip_gradients_min: Float, clip_gradients_max: Float, regularization_func: BNNSOptimizerRegularizationFunction)

Returns a new Adam optimizer fields structure from the specified parameters.

init()

Returns a new Adam optimizer fields structure.

### Instance Properties

var learning_rate: Float

A value that specifies the learning rate.

var beta1: Float

A value that specifies the first moment constant in the range 0 to 1.

var beta2: Float

A value that specifies the second moment constant in the range 0 to 1.

var time_step: Float

A value that represents the optimizer’s current time and you’re responsible for updating after optimizing all the layer parameters in your network.

var epsilon: Float

An addition for the division in the parameter update stage.

var gradient_scale: Float

A value that specifies the gradient scaling factor.

var regularization_scale: Float

A value that specifies the regularization scaling factor.

var clip_gradients: Bool

A Boolean value that specifies whether to clip the gradient between minimum and maximum values.

var clip_gradients_min: Float

The values for the minimum gradient.

var clip_gradients_max: Float

The values for the maximum gradient.

var regularization_func: BNNSOptimizerRegularizationFunction

The variable that specifies the regularization function.

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

