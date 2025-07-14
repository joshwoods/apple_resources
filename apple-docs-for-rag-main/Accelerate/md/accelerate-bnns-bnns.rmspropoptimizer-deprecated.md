

- Accelerate
- BNNS
-  BNNS.RMSPropOptimizer Deprecated

Structure

# BNNS.RMSPropOptimizer

An optimizer that uses the root mean square propagation (RMSProp) optimization method.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
struct RMSPropOptimizer
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Creating an RMSProp Optimizer

init(learningRate: Float, alpha: Float, epsilon: Float, centered: Bool, momentum: Float, gradientScale: Float, regularizationScale: Float, clipsGradientsTo: ClosedRange&lt;Float>?, regularizationFunction: BNNSOptimizerRegularizationFunction)

Returns a new RMSProp optimizer object.

init(learningRate: Float, alpha: Float, epsilon: Float, centered: Bool, momentum: Float, gradientScale: Float, regularizationScale: Float, gradientClipping: BNNS.GradientClipping, regularizationFunction: BNNSOptimizerRegularizationFunction)

Returns a new RMSProp optimizer object with gradient clipped by value or clipped by norm.

### Inspecting the Properties of an RMSProp Optimizer

var learningRate: Float

A value that specifies the learning rate.

var alpha: Float

A constant that specifies smoothing.

var epsilon: Float

A term that the optimizer adds to the denominator.

var centered: Bool

A Boolean value that specifies whether to use the centered variant.

var momentum: Float

The rate of momentum decay.

var gradientScale: Float

A value that specifies the gradient scaling factor.

var regularizationScale: Float

A value that specifies the regularization scaling factor.

var gradientBounds: ClosedRange&lt;Float>?

The values for the minimum and maximum gradients.

var gradientClipping: BNNS.GradientClipping

The gradient clipping.

enum GradientClipping

Constants that describe clipping functions.

var regularizationFunction: BNNSOptimizerRegularizationFunction

The variable that specifies the regularization function.

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

struct AdamWOptimizer

An optimizer that uses the AdamW optimization algorithm.

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

