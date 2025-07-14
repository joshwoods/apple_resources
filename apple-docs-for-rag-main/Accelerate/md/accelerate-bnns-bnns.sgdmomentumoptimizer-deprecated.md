

- Accelerate
- BNNS
-  BNNS.SGDMomentumOptimizer Deprecated

Structure

# BNNS.SGDMomentumOptimizer

An optimizer that uses the stochastic gradient descent (SGD) with the momentum optimization method.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+watchOS 7.0+visionOS

``` source
struct SGDMomentumOptimizer
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Creating an SGD with Momentum Optimizer

init(learningRate: Float, momentum: Float, gradientScale: Float, regularizationScale: Float, clipsGradientsTo: ClosedRange&lt;Float>?, usesNestrovMomentum: Bool, regularizationFunction: BNNSOptimizerRegularizationFunction, sgdMomentumVariant: BNNSOptimizerSGDMomentumVariant)

Returns a new stochastic gradient descent (SGD) with momentum optimizer object.

### Inspecting the Properties of an SGD with Momentum Optimizer

var learningRate: Float

A value that specifies the learning rate.

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

var usesNestrovMomentum: Bool

A Boolean value that specifies whether to use Nesterov momentum update.

var regularizationFunction: BNNSOptimizerRegularizationFunction

The variable that specifies the regularization function.

var sgdMomentumVariant: BNNSOptimizerSGDMomentumVariant

The variable that specifies the momentum variant.

var accumulatorCountMultiplier: Int

The number of accumulators required for each parameter.

### Initializers

init(learningRate: Float, momentum: Float, gradientScale: Float, regularizationScale: Float, clipsGradientsTo: ClosedRange&lt;Float>?, usesNesterovMomentum: Bool, regularizationFunction: BNNSOptimizerRegularizationFunction, sgdMomentumVariant: BNNSOptimizerSGDMomentumVariant)

init(learningRate: Float, momentum: Float, gradientScale: Float, regularizationScale: Float, gradientClipping: BNNS.GradientClipping, usesNesterovMomentum: Bool, regularizationFunction: BNNSOptimizerRegularizationFunction, sgdMomentumVariant: BNNSOptimizerSGDMomentumVariant)

### Instance Properties

var usesNesterovMomentum: Bool

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

struct RMSPropOptimizer

An optimizer that uses the root mean square propagation (RMSProp) optimization method.

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

