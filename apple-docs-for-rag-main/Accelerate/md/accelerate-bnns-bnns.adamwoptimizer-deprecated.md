

- Accelerate
- BNNS
-  BNNS.AdamWOptimizer Deprecated

Structure

# BNNS.AdamWOptimizer

An optimizer that uses the AdamW optimization algorithm.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+visionOSwatchOS 8.0+tvOS 15.0+

``` source
struct AdamWOptimizer
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Creating an AdamW Optimizer

init(learningRate: Float, beta1: Float, beta2: Float, timeStep: Float, epsilon: Float, gradientScale: Float, weightDecay: Float, gradientClipping: BNNS.GradientClipping, usesAMSGrad: Bool)

Returns a new AdamW optimizer object with gradient clipped by value or clipped by norm.

### Inspecting the Properties of an AdamW Optimizer

var learningRate: Float

A value that specifies the learning rate.

var beta1: Float

A value that specifies the first-moment constant, in the range `0` to `1`.

var beta2: Float

A value that specifies the second-moment constant, in the range `0` to `1`.

var timeStep: Float

A value that’s at least `1` and represents the optimizer’s current time.

var epsilon: Float

The epsilon value you use to improve numerical stability.

var gradientScale: Float

A value that specifies the gradient scaling factor.

var weightDecay: Float

The weight decay coefficient.

var gradientClipping: BNNS.GradientClipping

The gradient clipping function and bounds.

enum GradientClipping

Constants that describe clipping functions.

var accumulatorCountMultiplier: Int

The number of accumulators required for each parameter.

## Relationships

### Conforms To

- BNNSOptimizer

## See Also

### Optimizers

struct AdamOptimizer

An optimizer that uses the Adam optimization algorithm.

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

