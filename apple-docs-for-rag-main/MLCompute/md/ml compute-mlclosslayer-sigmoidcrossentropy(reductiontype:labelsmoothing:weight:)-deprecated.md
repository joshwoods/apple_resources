

- ML Compute
- MLCLossLayer
-  sigmoidCrossEntropy(reductionType:labelSmoothing:weight:) Deprecated

Type Method

# sigmoidCrossEntropy(reductionType:labelSmoothing:weight:)

Creates a sigmoid cross entropy loss layer with the reduction type, label smoothing, and weight you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class func sigmoidCrossEntropy(
    reductionType: MLCReductionType,
    labelSmoothing: Float,
    weight: Float
) -> Self
```

## Parameters 

`reductionType`  

The reduction operation type.

`labelSmoothing`  

The value for label smoothing.

`weight`  

A scalar floating-point weight value.

## Return Value

A sigmoid cross entropy loss layer.

## See Also

### Creating Loss Layers with Scalar Weights

class func softmaxCrossEntropy(reductionType: MLCReductionType, labelSmoothing: Float, classCount: Int, weight: Float) -> Self

Creates a softmax cross entropy loss layer with the reduction type, label smoothing, number of classes, and weight you specify.

Deprecated

class func categoricalCrossEntropy(reductionType: MLCReductionType, labelSmoothing: Float, classCount: Int, weight: Float) -> Self

Creates a categorical cross entropy loss layer with the reduction type, label smoothing, number of classes, and weight you specify.

Deprecated

class func log(reductionType: MLCReductionType, epsilon: Float, weight: Float) -> Self

Creates a log loss layer with the reduction type, epsilon, and weight you specify.

Deprecated

class func huberLoss(reductionType: MLCReductionType, delta: Float, weight: Float) -> Self

Creates a huber loss layer with the reduction type, delta, and weight you specify.

Deprecated

class func meanAbsoluteError(reductionType: MLCReductionType, weight: Float) -> Self

Creates a mean absolute loss layer with the reduction type and weight.

Deprecated

class func meanSquaredError(reductionType: MLCReductionType, weight: Float) -> Self

Creates a mean squared loss layer with the reduction type and weight you specify.

Deprecated

class func hingeLoss(reductionType: MLCReductionType, weight: Float) -> Self

Creates a hinge loss layer with the reduction type and weight you specify.

Deprecated

class func cosineDistance(reductionType: MLCReductionType, weight: Float) -> Self

Creates a cosine distance loss layer with the reduction type and weight you specify.

Deprecated

