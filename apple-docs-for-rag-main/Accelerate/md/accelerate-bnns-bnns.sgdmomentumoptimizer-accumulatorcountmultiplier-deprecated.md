

- Accelerate
- BNNS
- BNNS.SGDMomentumOptimizer
-  accumulatorCountMultiplier Deprecated

Instance Property

# accumulatorCountMultiplier

The number of accumulators required for each parameter.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
var accumulatorCountMultiplier: Int { get }
```

Deprecated

Use the BNNSGraph API instead.

## See Also

### Inspecting the Properties of an SGD with Momentum Optimizer

var learningRate: Float

A value that specifies the learning rate.

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

var usesNestrovMomentum: Bool

A Boolean value that specifies whether to use Nesterov momentum update.

Deprecated

var regularizationFunction: BNNSOptimizerRegularizationFunction

The variable that specifies the regularization function.

Deprecated

var sgdMomentumVariant: BNNSOptimizerSGDMomentumVariant

The variable that specifies the momentum variant.

Deprecated

