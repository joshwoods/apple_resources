

- Accelerate
- BNNS
- BNNS.LossFunction
-  BNNS.LossFunction.huber(huberDelta:) Deprecated

Case

# BNNS.LossFunction.huber(huberDelta:)

Huber loss computation between input logits and one-hot encoded labels.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
case huber(huberDelta: Float)
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

case yolo(parameters: BNNS.LossFunction.YoloParameters)

You Only Look Once (YOLO) loss computation between prediction and ground truth labels.

Deprecated

struct YoloParameters

A structure that contains the parameters for You Only Look Once (YOLO) loss computation.

Deprecated

