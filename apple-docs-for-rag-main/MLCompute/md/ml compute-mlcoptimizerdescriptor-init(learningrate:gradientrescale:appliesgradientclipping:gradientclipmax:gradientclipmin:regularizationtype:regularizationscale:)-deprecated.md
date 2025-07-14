

- ML Compute
- MLCOptimizerDescriptor
-  init(learningRate:gradientRescale:appliesGradientClipping:gradientClipMax:gradientClipMin:regularizationType:regularizationScale:) Deprecated

Initializer

# init(learningRate:gradientRescale:appliesGradientClipping:gradientClipMax:gradientClipMin:regularizationType:regularizationScale:)

Creates a descriptor with the learning rate, gradient rescale, clipping option and values, and regularization type and scale that you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
convenience init(
    learningRate: Float,
    gradientRescale: Float,
    appliesGradientClipping: Bool,
    gradientClipMax: Float,
    gradientClipMin: Float,
    regularizationType: MLCRegularizationType,
    regularizationScale: Float
)
```

## Parameters 

`learningRate`  

The learning rate.

`gradientRescale`  

The gradient rescale value.

`appliesGradientClipping`  

A Boolean value that indicates whether you apply gradient clipping.

`gradientClipMax`  

The maximum gradient value before the optimizer rescales the gradient, if you enable gradient clipping.

`gradientClipMin`  

The minimum gradient value before the optimizer rescales the gradient, if you enable gradient clipping.

`regularizationType`  

The regularization type.

`regularizationScale`  

The regularization scale.

## See Also

### Creating an Optimizer Descriptor

convenience init(learningRate: Float, gradientRescale: Float, regularizationType: MLCRegularizationType, regularizationScale: Float)

Creates an optimizer descriptor with the learning rate, gradient rescale, regularization type, and regulation scale that you specify.

Deprecated

convenience init(learningRate: Float, gradientRescale: Float, appliesGradientClipping: Bool, gradientClippingType: MLCGradientClippingType, gradientClipMax: Float, gradientClipMin: Float, maximumClippingNorm: Float, customGlobalNorm: Float, regularizationType: MLCRegularizationType, regularizationScale: Float)

Creates a descriptor with the learning rate, gradient rescale, clipping option and values, and regularization type and scale that you specify.

Deprecated

