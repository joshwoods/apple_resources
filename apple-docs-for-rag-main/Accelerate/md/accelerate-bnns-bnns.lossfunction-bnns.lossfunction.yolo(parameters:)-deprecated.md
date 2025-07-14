

- Accelerate
- BNNS
- BNNS.LossFunction
-  BNNS.LossFunction.yolo(parameters:) Deprecated

Case

# BNNS.LossFunction.yolo(parameters:)

You Only Look Once (YOLO) loss computation between prediction and ground truth labels.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+watchOS 7.0+visionOS

``` source
case yolo(parameters: BNNS.LossFunction.YoloParameters)
```

Deprecated

Use the BNNSGraph API instead.

## See Also

### Loss Functions

case categoricalCrossEntropy

Categorical cross-entropy computation between input prediction and labels.

Deprecated

case cosineDistance

Cosine distance loss computation between input predictions and labels.

Deprecated

case hinge

Hinge loss computation between labels and unbounded, zero-centered binary predictions.

Deprecated

case huber(huberDelta: Float)

Huber loss computation between input logits and one-hot encoded labels.

Deprecated

case log

Log loss computation between labels and predictions.

Deprecated

case meanAbsoluteError

Mean absolute error (MAE) computation between input prediction and labels.

Deprecated

case meanSquareError

Mean square error (MSE) computation between input logits and one-hot encoded labels.

Deprecated

case sigmoidCrossEntropy(labelSmoothing: Float)

Sigmoid activation on input logits, and independent computation of cross-entropy loss for each class.

Deprecated

case softmaxCrossEntropy(labelSmoothing: Float)

Softmax activation on input logits, and computation of cross-entropy loss with one-hot encoded labels.

Deprecated

struct YoloParameters

A structure that contains the parameters for You Only Look Once (YOLO) loss computation.

Deprecated

