

- Accelerate
- BNNS
- BNNS.AdamOptimizer
-  init(learningRate:beta1:beta2:timeStep:epsilon:gradientScale:regularizationScale:gradientClipping:regularizationFunction:usesAMSGrad:) Deprecated

Initializer

# init(learningRate:beta1:beta2:timeStep:epsilon:gradientScale:regularizationScale:gradientClipping:regularizationFunction:usesAMSGrad:)

Returns a new Adam optimizer object with gradient clipped by value or clipped by norm.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+Mac Catalyst

``` source
init(
    learningRate: Float = 0.001,
    beta1: Float = 0.9,
    beta2: Float = 0.999,
    timeStep: Float,
    epsilon: Float = 1e-8,
    gradientScale: Float,
    regularizationScale: Float,
    gradientClipping: BNNS.GradientClipping,
    regularizationFunction: BNNSOptimizerRegularizationFunction,
    usesAMSGrad: Bool = false
)
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`learningRate`  

A value that specifies the learning rate.

`beta1`  

A value that specifies the first-moment constant, in the range `0` to `1`.

`beta2`  

A value that specifies the second-moment constant, in the range `0` to `1`.

`timeStep`  

A value that’s at least `1` and represents the optimizer’s current time.

`epsilon`  

The epsilon value you use to improve numerical stability.

`gradientScale`  

A value that specifies the gradient scaling factor.

`regularizationScale`  

A value that specifies the regularization scaling factor.

`gradientClipping`  

The gradient clipping function and bounds.

`regularizationFunction`  

A value that specifies the regularization function.

`usesAMSGrad`  

A Boolean value that specifies whether the optimizer should use the AMSGrad variant.

## See Also

### Creating an Adam Optimizer

init(learningRate: Float, beta1: Float, beta2: Float, timeStep: Float, epsilon: Float, gradientScale: Float, regularizationScale: Float, clipsGradientsTo: ClosedRange&lt;Float>?, regularizationFunction: BNNSOptimizerRegularizationFunction)

Returns a new Adam optimizer object.

Deprecated

