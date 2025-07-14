

- Accelerate
- BNNS
- BNNS.SGDMomentumOptimizer
-  gradientClipping 

Instance Property

# gradientClipping

The gradient clipping.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
var gradientClipping: BNNS.GradientClipping { get set }
```

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

var accumulatorCountMultiplier: Int

The number of accumulators required for each parameter.

Deprecated

