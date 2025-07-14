

- Accelerate
- BNNS
- BNNS.SGDMomentumOptimizer
-  init(learningRate:momentum:gradientScale:regularizationScale:clipsGradientsTo:usesNestrovMomentum:regularizationFunction:sgdMomentumVariant:) 

Initializer

# init(learningRate:momentum:gradientScale:regularizationScale:clipsGradientsTo:usesNestrovMomentum:regularizationFunction:sgdMomentumVariant:)

Returns a new stochastic gradient descent (SGD) with momentum optimizer object.

iOS 14.0–15.0DeprecatediPadOS 14.0–15.0DeprecatedMac CatalystmacOS 11.0–12.0DeprecatedtvOS 14.0–15.0DeprecatedvisionOSwatchOS 7.0–8.0Deprecated

``` source
init(
    learningRate: Float,
    momentum: Float,
    gradientScale: Float,
    regularizationScale: Float,
    clipsGradientsTo gradientBounds: ClosedRange? = nil,
    usesNestrovMomentum: Bool,
    regularizationFunction: BNNSOptimizerRegularizationFunction,
    sgdMomentumVariant: BNNSOptimizerSGDMomentumVariant
)
```

## Parameters 

`learningRate`  

A value that specifies the learning rate.

`momentum`  

The rate of momentum decay.

`gradientScale`  

A value that specifies the gradient scaling factor.

`regularizationScale`  

A value that specifies the regularization scaling factor.

`gradientBounds`  

The values for the minimum and maximum gradients.

`usesNestrovMomentum`  

A Boolean value that specifies whether to use Nesterov momentum update.

`regularizationFunction`  

The variable that specifies the regularization function.

`sgdMomentumVariant`  

The variable that specifies the momentum variant.

