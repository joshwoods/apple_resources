

- Accelerate
- BNNS
- BNNS.AdamWOptimizer
-  weightDecay Deprecated

Instance Property

# weightDecay

The weight decay coefficient.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+Mac Catalyst

``` source
var weightDecay: Float { get set }
```

Deprecated

Use the BNNSGraph API instead.

## See Also

### Inspecting the Properties of an AdamW Optimizer

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

var gradientClipping: BNNS.GradientClipping

The gradient clipping function and bounds.

Deprecated

enum GradientClipping

Constants that describe clipping functions.

var accumulatorCountMultiplier: Int

The number of accumulators required for each parameter.

Deprecated

