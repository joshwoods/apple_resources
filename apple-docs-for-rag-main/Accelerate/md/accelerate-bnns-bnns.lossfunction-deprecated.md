

- Accelerate
- BNNS
-  BNNS.LossFunction Deprecated

Enumeration

# BNNS.LossFunction

Constants that describe loss functions.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOSwatchOS 7.0+tvOS 14.0+

``` source
enum LossFunction
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Loss Functions

case categoricalCrossEntropy

Categorical cross-entropy computation between input prediction and labels.

case cosineDistance

Cosine distance loss computation between input predictions and labels.

case hinge

Hinge loss computation between labels and unbounded, zero-centered binary predictions.

case huber(huberDelta: Float)

Huber loss computation between input logits and one-hot encoded labels.

case log

Log loss computation between labels and predictions.

case meanAbsoluteError

Mean absolute error (MAE) computation between input prediction and labels.

case meanSquareError

Mean square error (MSE) computation between input logits and one-hot encoded labels.

case sigmoidCrossEntropy(labelSmoothing: Float)

Sigmoid activation on input logits, and independent computation of cross-entropy loss for each class.

case softmaxCrossEntropy(labelSmoothing: Float)

Softmax activation on input logits, and computation of cross-entropy loss with one-hot encoded labels.

case yolo(parameters: BNNS.LossFunction.YoloParameters)

You Only Look Once (YOLO) loss computation between prediction and ground truth labels.

struct YoloParameters

A structure that contains the parameters for You Only Look Once (YOLO) loss computation.

### Instance Properties

var bnnsLossFunction: BNNSLossFunction

The underlying loss function structure.

