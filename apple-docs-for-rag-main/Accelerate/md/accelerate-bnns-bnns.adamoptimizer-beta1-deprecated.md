

- Accelerate
- BNNS
- BNNS.AdamOptimizer
-  beta1 Deprecated

Instance Property

# beta1

A value that specifies the first-moment constant, in the range `0` to `1`.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
var beta1: Float { get set }
```

Deprecated

Use the BNNSGraph API instead.

## See Also

### Inspecting the Properties of an Adam Optimizer

var learningRate: Float

A value that specifies the learning rate.

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

enum GradientClipping

Constants that describe clipping functions.

