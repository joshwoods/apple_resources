

- Accelerate
-  BNNSLossFunctionSoftmaxCrossEntropy 

Global Variable

# BNNSLossFunctionSoftmaxCrossEntropy

Softmax activation on input logits, and computation of cross-entropy loss with one-hot encoded labels.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var BNNSLossFunctionSoftmaxCrossEntropy: BNNSLossFunction { get }
```

## Discussion

BNNSLossFunctionSoftmaxCrossEntropy performs softmax on input logits and computes cross entropy loss with one hot encoded labels.

You can smooth labels can according to smoothing factor.

You can scale the loss with either a scalar value or weight matrix, and reduce the loss according to a reduction function.

## See Also

### Loss Functions

init(UInt32)

init(rawValue: UInt32)

var rawValue: UInt32

var BNNSLossFunctionCategoricalCrossEntropy: BNNSLossFunction

Performs categorical cross entropy computation between input prediction and labels.

var BNNSLossFunctionCosineDistance: BNNSLossFunction

Performs cosine distance loss computation between input predictions and labels.

var BNNSLossFunctionHinge: BNNSLossFunction

Performs Hinge loss computation between labels and unbounded zero-centered binary predictions.

var BNNSLossFunctionHuber: BNNSLossFunction

Huber loss computation between input logits and one-hot encoded labels.

var BNNSLossFunctionLog: BNNSLossFunction

Log loss computation between labels and predictions.

var BNNSLossFunctionMeanAbsoluteError: BNNSLossFunction

Mean absolute error (MAE) computation between input prediction and labels.

var BNNSLossFunctionMeanSquareError: BNNSLossFunction

Mean square error (MSE) computation between input logits and one-hot encoded labels.

var BNNSLossFunctionSigmoidCrossEntropy: BNNSLossFunction

Sigmoid activation on input logits, and independent computation of cross-entropy loss for each class.

var BNNSLossFunctionYolo: BNNSLossFunction

You Only Look Once (YOLO) loss computation between prediction and ground truth labels.

