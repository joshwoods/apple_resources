

- Accelerate
- BNNS
-  BNNS.AdamOptimizer Deprecated

Structure

# BNNS.AdamOptimizer

An optimizer that uses the Adam optimization algorithm.

iOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+Mac Catalyst

``` source
struct AdamOptimizer
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Creating an Adam Optimizer

init(learningRate: Float, beta1: Float, beta2: Float, timeStep: Float, epsilon: Float, gradientScale: Float, regularizationScale: Float, clipsGradientsTo: ClosedRange&lt;Float>?, regularizationFunction: BNNSOptimizerRegularizationFunction)

Returns a new Adam optimizer object.

init(learningRate: Float, beta1: Float, beta2: Float, timeStep: Float, epsilon: Float, gradientScale: Float, regularizationScale: Float, gradientClipping: BNNS.GradientClipping, regularizationFunction: BNNSOptimizerRegularizationFunction, usesAMSGrad: Bool)

Returns a new Adam optimizer object with gradient clipped by value or clipped by norm.

### Inspecting the Properties of an Adam Optimizer

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

var regularizationScale: Float

A value that specifies the regularization scaling factor.

var gradientBounds: ClosedRange&lt;Float>?

The values for the minimum and maximum gradients.

var gradientClipping: BNNS.GradientClipping

The gradient clipping.

var regularizationFunction: BNNSOptimizerRegularizationFunction

The variable that specifies the regularization function.

var usesAMSGrad: Bool

A Boolean value that specifies whether to use the AMSGrad variant.

var accumulatorCountMultiplier: Int

The number of accumulators required for each parameter.

enum GradientClipping

Constants that describe clipping functions.

## Relationships

### Conforms To

- BNNSOptimizer

## See Also

### Optimizers

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

