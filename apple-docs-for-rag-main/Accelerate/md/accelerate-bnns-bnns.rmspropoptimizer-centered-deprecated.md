

- Accelerate
- BNNS
- BNNS.RMSPropOptimizer
-  centered Deprecated

Instance Property

# centered

A Boolean value that specifies whether to use the centered variant.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
var centered: Bool { get set }
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

