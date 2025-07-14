

- Accelerate
- BNNS
- BNNS.SGDMomentumOptimizer
-  init(learningRate:momentum:gradientScale:regularizationScale:gradientClipping:usesNesterovMomentum:regularizationFunction:sgdMomentumVariant:) 

Initializer

# init(learningRate:momentum:gradientScale:regularizationScale:gradientClipping:usesNesterovMomentum:regularizationFunction:sgdMomentumVariant:)

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
init(
    learningRate: Float,
    momentum: Float = 0,
    gradientScale: Float,
    regularizationScale: Float,
    gradientClipping: BNNS.GradientClipping,
    usesNesterovMomentum: Bool = false,
    regularizationFunction: BNNSOptimizerRegularizationFunction,
    sgdMomentumVariant: BNNSOptimizerSGDMomentumVariant
)
```

