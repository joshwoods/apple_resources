

- ML Compute
- MLCLossLayer
-  cosineDistance(reductionType:weights:) Deprecated

Type Method

# cosineDistance(reductionType:weights:)

Creates a cosine distance loss layer with the reduction type and weights you specify.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class func cosineDistance(
    reductionType: MLCReductionType,
    weights: MLCTensor?
) -> Self
```

## Parameters 

`reductionType`  

The reduction operation type.

`weights`  

The loss label weights tensor.

## Return Value

A cosine distance loss layer.

## See Also

### Creating Loss Layers with Tensor Weights

class func softmaxCrossEntropy(reductionType: MLCReductionType, labelSmoothing: Float, classCount: Int, weights: MLCTensor?) -> Self

Creates a softmax cross entropy loss layer with the reduction type, label smoothing, number of classes, and weights you specify.

Deprecated

class func categoricalCrossEntropy(reductionType: MLCReductionType, labelSmoothing: Float, classCount: Int, weights: MLCTensor?) -> Self

Creates a categorical cross entropy loss layer with the reduction type, label smoothing, number of classes, and weights you specify.

Deprecated

class func sigmoidCrossEntropy(reductionType: MLCReductionType, labelSmoothing: Float, weights: MLCTensor?) -> Self

Creates a sigmoid cross entropy loss layer with the reduction type, label smoothing, and weights you specify.

Deprecated

class func log(reductionType: MLCReductionType, epsilon: Float, weights: MLCTensor?) -> Self

Creates a log loss layer with the reduction type, epsilon, and weights you specify.

Deprecated

class func huberLoss(reductionType: MLCReductionType, delta: Float, weights: MLCTensor?) -> Self

Creates a huber loss layer with the reduction type, delta, and weights you specify.

Deprecated

class func meanAbsoluteError(reductionType: MLCReductionType, weights: MLCTensor?) -> Self

Creates a mean absolute loss layer with the reduction type and weights you specify.

Deprecated

class func meanSquaredError(reductionType: MLCReductionType, weights: MLCTensor?) -> Self

Creates a mean squared loss layer with the reduction type and weights you specify.

Deprecated

class func hingeLoss(reductionType: MLCReductionType, weights: MLCTensor?) -> Self

Creates a hinge loss layer with the reduction type and weights you specify.

Deprecated

