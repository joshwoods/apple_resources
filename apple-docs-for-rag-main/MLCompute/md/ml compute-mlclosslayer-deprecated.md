

- ML Compute
-  MLCLossLayer Deprecated

Class

# MLCLossLayer

A layer that estimates the inaccuracies of the model to reduce the loss on the next evaluation.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCLossLayer
```

## Topics

### Creating Loss Layers with Descriptors

convenience init(descriptor: MLCLossDescriptor)

Creates a loss layer with the descriptor you specify.

convenience init(descriptor: MLCLossDescriptor, weights: MLCTensor)

Creates a loss layer with the descriptor and weights you specify.

class MLCLossDescriptor

A configuration object you use to create a loss layer.

enum MLCLossType

A loss function.

### Creating Loss Layers with Scalar Weights

class func softmaxCrossEntropy(reductionType: MLCReductionType, labelSmoothing: Float, classCount: Int, weight: Float) -> Self

Creates a softmax cross entropy loss layer with the reduction type, label smoothing, number of classes, and weight you specify.

class func categoricalCrossEntropy(reductionType: MLCReductionType, labelSmoothing: Float, classCount: Int, weight: Float) -> Self

Creates a categorical cross entropy loss layer with the reduction type, label smoothing, number of classes, and weight you specify.

class func sigmoidCrossEntropy(reductionType: MLCReductionType, labelSmoothing: Float, weight: Float) -> Self

Creates a sigmoid cross entropy loss layer with the reduction type, label smoothing, and weight you specify.

class func log(reductionType: MLCReductionType, epsilon: Float, weight: Float) -> Self

Creates a log loss layer with the reduction type, epsilon, and weight you specify.

class func huberLoss(reductionType: MLCReductionType, delta: Float, weight: Float) -> Self

Creates a huber loss layer with the reduction type, delta, and weight you specify.

class func meanAbsoluteError(reductionType: MLCReductionType, weight: Float) -> Self

Creates a mean absolute loss layer with the reduction type and weight.

class func meanSquaredError(reductionType: MLCReductionType, weight: Float) -> Self

Creates a mean squared loss layer with the reduction type and weight you specify.

class func hingeLoss(reductionType: MLCReductionType, weight: Float) -> Self

Creates a hinge loss layer with the reduction type and weight you specify.

class func cosineDistance(reductionType: MLCReductionType, weight: Float) -> Self

Creates a cosine distance loss layer with the reduction type and weight you specify.

### Creating Loss Layers with Tensor Weights

class func softmaxCrossEntropy(reductionType: MLCReductionType, labelSmoothing: Float, classCount: Int, weights: MLCTensor?) -> Self

Creates a softmax cross entropy loss layer with the reduction type, label smoothing, number of classes, and weights you specify.

class func categoricalCrossEntropy(reductionType: MLCReductionType, labelSmoothing: Float, classCount: Int, weights: MLCTensor?) -> Self

Creates a categorical cross entropy loss layer with the reduction type, label smoothing, number of classes, and weights you specify.

class func sigmoidCrossEntropy(reductionType: MLCReductionType, labelSmoothing: Float, weights: MLCTensor?) -> Self

Creates a sigmoid cross entropy loss layer with the reduction type, label smoothing, and weights you specify.

class func log(reductionType: MLCReductionType, epsilon: Float, weights: MLCTensor?) -> Self

Creates a log loss layer with the reduction type, epsilon, and weights you specify.

class func huberLoss(reductionType: MLCReductionType, delta: Float, weights: MLCTensor?) -> Self

Creates a huber loss layer with the reduction type, delta, and weights you specify.

class func meanAbsoluteError(reductionType: MLCReductionType, weights: MLCTensor?) -> Self

Creates a mean absolute loss layer with the reduction type and weights you specify.

class func meanSquaredError(reductionType: MLCReductionType, weights: MLCTensor?) -> Self

Creates a mean squared loss layer with the reduction type and weights you specify.

class func hingeLoss(reductionType: MLCReductionType, weights: MLCTensor?) -> Self

Creates a hinge loss layer with the reduction type and weights you specify.

class func cosineDistance(reductionType: MLCReductionType, weights: MLCTensor?) -> Self

Creates a cosine distance loss layer with the reduction type and weights you specify.

### Inspecting Loss Layers

var descriptor: MLCLossDescriptor

The configuration object you use to create the loss layer.

var weights: MLCTensor?

The loss label weights tensor.

## Relationships

### Inherits From

- MLCLayer

### Inherited By

- MLCYOLOLossLayer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Loss Layers

class MLCYOLOLossLayer

A layer that estimates loss for the YOLO algorithm.

Deprecated

