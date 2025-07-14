

- Accelerate
- BNNS
- BNNS.SGDMomentumOptimizer
-  usesNestrovMomentum 

Instance Property

# usesNestrovMomentum

A Boolean value that specifies whether to use Nesterov momentum update.

iOS 14.0–15.0DeprecatediPadOS 14.0–15.0DeprecatedMac CatalystmacOS 11.0–12.0DeprecatedtvOS 14.0–15.0DeprecatedvisionOSwatchOS 7.0–8.0Deprecated

``` source
var usesNestrovMomentum: Bool { get set }
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

var gradientClipping: BNNS.GradientClipping

The gradient clipping.

enum GradientClipping

Constants that describe clipping functions.

var regularizationFunction: BNNSOptimizerRegularizationFunction

The variable that specifies the regularization function.

Deprecated

var sgdMomentumVariant: BNNSOptimizerSGDMomentumVariant

The variable that specifies the momentum variant.

Deprecated

var accumulatorCountMultiplier: Int

The number of accumulators required for each parameter.

Deprecated

