

- Accelerate
- BNNS
- BNNS.RMSPropOptimizer
-  init(learningRate:alpha:epsilon:centered:momentum:gradientScale:regularizationScale:clipsGradientsTo:regularizationFunction:) Deprecated

Initializer

# init(learningRate:alpha:epsilon:centered:momentum:gradientScale:regularizationScale:clipsGradientsTo:regularizationFunction:)

Returns a new RMSProp optimizer object.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+watchOS 7.0+visionOS

``` source
init(
    learningRate: Float,
    alpha: Float,
    epsilon: Float,
    centered: Bool,
    momentum: Float,
    gradientScale: Float,
    regularizationScale: Float,
    clipsGradientsTo gradientBounds: ClosedRange? = nil,
    regularizationFunction: BNNSOptimizerRegularizationFunction
)
```

Deprecated

Use the BNNSGraph API instead.

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

`gradientBounds`  

The values for the minimum and maximum gradients.

`regularizationFunction`  

The variable that specifies the regularization function.

## See Also

### Creating an RMSProp Optimizer

init(learningRate: Float, alpha: Float, epsilon: Float, centered: Bool, momentum: Float, gradientScale: Float, regularizationScale: Float, gradientClipping: BNNS.GradientClipping, regularizationFunction: BNNSOptimizerRegularizationFunction)

Returns a new RMSProp optimizer object with gradient clipped by value or clipped by norm.

