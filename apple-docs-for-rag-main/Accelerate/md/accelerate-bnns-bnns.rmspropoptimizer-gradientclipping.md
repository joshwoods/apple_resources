

- Accelerate
- BNNS
- BNNS.RMSPropOptimizer
-  gradientClipping 

Instance Property

# gradientClipping

The gradient clipping.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
var gradientClipping: BNNS.GradientClipping { get set }
```

## See Also

### Inspecting the Properties of an RMSProp Optimizer

var learningRate: Float

A value that specifies the learning rate.

Deprecated

var alpha: Float

A constant that specifies smoothing.

Deprecated

var epsilon: Float

A term that the optimizer adds to the denominator.

Deprecated

var centered: Bool

A Boolean value that specifies whether to use the centered variant.

Deprecated

var momentum: Float

The rate of momentum decay.

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

enum GradientClipping

Constants that describe clipping functions.

var regularizationFunction: BNNSOptimizerRegularizationFunction

The variable that specifies the regularization function.

Deprecated

var accumulatorCountMultiplier: Int

The number of accumulators required for each parameter.

Deprecated

