

- Accelerate
- BNNS
- BNNS.RMSPropOptimizer
-  init(learningRate:alpha:epsilon:centered:momentum:gradientScale:regularizationScale:gradientClipping:regularizationFunction:) 

Initializer

# init(learningRate:alpha:epsilon:centered:momentum:gradientScale:regularizationScale:gradientClipping:regularizationFunction:)

Returns a new RMSProp optimizer object with gradient clipped by value or clipped by norm.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
init(
    learningRate: Float = 1e-2,
    alpha: Float = 0.99,
    epsilon: Float = 1e-8,
    centered: Bool,
    momentum: Float = 0,
    gradientScale: Float,
    regularizationScale: Float,
    gradientClipping: BNNS.GradientClipping,
    regularizationFunction: BNNSOptimizerRegularizationFunction
)
```

## Parameters 

`learningRate`  

A value that specifies the learning rate.

`alpha`  

A constant that specifies smoothing, in the range `0` to `1`.

`epsilon`  

A term that the optimizer adds to the denominator.

`centered`  

A Boolean value that specifies whether to use the centered variant.

`momentum`  

The rate of momentum decay.

`gradientScale`  

A value that specifies the gradient scaling factor.

`regularizationScale`  

A value that specifies the regularization scaling factor.

`gradientClipping`  

The gradient clipping function and bounds.

`regularizationFunction`  

The variable that specifies the regularization function.

## See Also

### Creating an RMSProp Optimizer

init(learningRate: Float, alpha: Float, epsilon: Float, centered: Bool, momentum: Float, gradientScale: Float, regularizationScale: Float, clipsGradientsTo: ClosedRange&lt;Float>?, regularizationFunction: BNNSOptimizerRegularizationFunction)

Returns a new RMSProp optimizer object.

Deprecated

