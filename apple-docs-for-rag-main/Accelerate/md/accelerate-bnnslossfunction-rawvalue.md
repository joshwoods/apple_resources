

- Accelerate
- BNNSLossFunction
-  rawValue 

Instance Property

# rawValue

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var rawValue: UInt32
```

## See Also

### Loss Functions

init(UInt32)

init(rawValue: UInt32)

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

var BNNSLossFunctionSoftmaxCrossEntropy: BNNSLossFunction

Softmax activation on input logits, and computation of cross-entropy loss with one-hot encoded labels.

var BNNSLossFunctionYolo: BNNSLossFunction

You Only Look Once (YOLO) loss computation between prediction and ground truth labels.

