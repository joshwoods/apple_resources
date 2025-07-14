

- Accelerate
- BNNS
- BNNS.AdamOptimizer
-  gradientClipping Deprecated

Instance Property

# gradientClipping

The gradient clipping.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+visionOSwatchOS 8.0+tvOS 15.0+

``` source
var gradientClipping: BNNS.GradientClipping { get set }
```

Deprecated

Use the BNNSGraph API instead.

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

