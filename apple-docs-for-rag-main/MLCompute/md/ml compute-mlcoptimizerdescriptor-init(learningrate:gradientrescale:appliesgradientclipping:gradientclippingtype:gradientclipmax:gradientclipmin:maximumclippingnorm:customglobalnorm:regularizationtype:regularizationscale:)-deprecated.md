

- ML Compute
- MLCOptimizerDescriptor
-  init(learningRate:gradientRescale:appliesGradientClipping:gradientClippingType:gradientClipMax:gradientClipMin:maximumClippingNorm:customGlobalNorm:regularizationType:regularizationScale:) Deprecated

Initializer

# init(learningRate:gradientRescale:appliesGradientClipping:gradientClippingType:gradientClipMax:gradientClipMin:maximumClippingNorm:customGlobalNorm:regularizationType:regularizationScale:)

Creates a descriptor with the learning rate, gradient rescale, clipping option and values, and regularization type and scale that you specify.

iOS 15.0–17.4DeprecatediPadOS 15.0–17.4DeprecatedMac Catalyst 15.0–17.4DeprecatedmacOS 12.0–14.3DeprecatedtvOS 15.0–17.4Deprecated

``` source
convenience init(
    learningRate: Float,
    gradientRescale: Float,
    appliesGradientClipping: Bool,
    gradientClippingType: MLCGradientClippingType,
    gradientClipMax: Float,
    gradientClipMin: Float,
    maximumClippingNorm: Float,
    customGlobalNorm: Float,
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

`gradientClippingType`  

The type of clipping the system applies to gradients.

`gradientClipMax`  

The maximum gradient value before the optimizer rescales the gradient, if you enable gradient clipping.

`gradientClipMin`  

The minimum gradient value before the optimizer rescales the gradient, if you enable gradient clipping.

`maximumClippingNorm`  

The maximum norm to use with gradient clipping.

`customGlobalNorm`  

If nonzero, the value the system uses instead of calculating it.

`regularizationType`  

The regularization type.

`regularizationScale`  

The regularization scale.

## See Also

### Creating an Optimizer Descriptor

convenience init(learningRate: Float, gradientRescale: Float, regularizationType: MLCRegularizationType, regularizationScale: Float)

Creates an optimizer descriptor with the learning rate, gradient rescale, regularization type, and regulation scale that you specify.

Deprecated

convenience init(learningRate: Float, gradientRescale: Float, appliesGradientClipping: Bool, gradientClipMax: Float, gradientClipMin: Float, regularizationType: MLCRegularizationType, regularizationScale: Float)

Creates a descriptor with the learning rate, gradient rescale, clipping option and values, and regularization type and scale that you specify.

Deprecated

