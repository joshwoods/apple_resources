

- Accelerate
- BNNS
- BNNS.RMSPropOptimizer
-  gradientBounds Deprecated

Instance Property

# gradientBounds

The values for the minimum and maximum gradients.

iOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+Mac Catalyst

``` source
var gradientBounds: ClosedRange? { get set }
```

Deprecated

Use the BNNSGraph API instead.

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

var gradientClipping: BNNS.GradientClipping

The gradient clipping.

enum GradientClipping

Constants that describe clipping functions.

var regularizationFunction: BNNSOptimizerRegularizationFunction

The variable that specifies the regularization function.

Deprecated

var accumulatorCountMultiplier: Int

The number of accumulators required for each parameter.

Deprecated

