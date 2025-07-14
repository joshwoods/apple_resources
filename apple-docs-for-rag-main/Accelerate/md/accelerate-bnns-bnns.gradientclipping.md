

- Accelerate
- BNNS
-  BNNS.GradientClipping 

Enumeration

# BNNS.GradientClipping

Constants that describe clipping functions.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
enum GradientClipping
```

## Topics

### Gradient Clipping Functions

case none

A constant that indicates that the operation doesn’t clip gradients.

case byValue(bounds: ClosedRange&lt;Float>)

A constant that indicates that the operation clips gradients to a specified range.

case byNorm(threshold: Float)

A constant that indicates that the operation clips gradients to a specified Euclidean norm.

case byGlobalNorm(threshold: Float, globalNorm: Float)

A constant that indicates that the operation clips gradients to a specified global Euclidean norm.

## See Also

### Inspecting the Properties of an Adam Optimizer

var learningRate: Float

A value that specifies the learning rate.

Deprecated

var beta1: Float

A value that specifies the first-moment constant, in the range `0` to `1`.

Deprecated

var beta2: Float

A value that specifies the second-moment constant, in the range `0` to `1`.

Deprecated

var timeStep: Float

A value that’s at least `1` and represents the optimizer’s current time.

Deprecated

var epsilon: Float

The epsilon value you use to improve numerical stability.

Deprecated

var gradientScale: Float

A value that specifies the gradient scaling factor.

Deprecated

var regularizationScale: Float

A value that specifies the regularization scaling factor.

Deprecated

var gradientBounds: ClosedRange&lt;Float>?

The values for the minimum and maximum gradients.

Deprecated

var gradientClipping: BNNS.GradientClipping

The gradient clipping.

Deprecated

var regularizationFunction: BNNSOptimizerRegularizationFunction

The variable that specifies the regularization function.

Deprecated

var usesAMSGrad: Bool

A Boolean value that specifies whether to use the AMSGrad variant.

Deprecated

var accumulatorCountMultiplier: Int

The number of accumulators required for each parameter.

Deprecated

