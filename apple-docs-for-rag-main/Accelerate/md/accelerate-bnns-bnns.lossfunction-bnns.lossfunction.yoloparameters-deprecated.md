

- Accelerate
- BNNS
- BNNS.LossFunction
-  BNNS.LossFunction.YoloParameters Deprecated

Structure

# BNNS.LossFunction.YoloParameters

A structure that contains the parameters for You Only Look Once (YOLO) loss computation.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+watchOS 7.0+visionOS

``` source
struct YoloParameters
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Instance Properties

let anchorBoxCount: Int

The number of anchor boxes in each cell.

let anchorBoxSize: Int

The size of the anchor box.

let anchorsData: UnsafeMutablePointer&lt;Float>

Maximum IOU for treating as no object.

let classificationScale: Float

The value that specifies the classification scaling factor.

let gridColumnCount: Int

The number of columns in the grid.

let gridRowsCount: Int

The number of rows in the grid.

let huberDelta: Float

A value that’s interpreted as width-height loss.

let noObjectMaximumIoU: Float

The value that specifies intersection over union (IOU) that’s the maximum the function treats as not an object.

let noObjectScale: Float

The value that specifies the no-object confidence scaling factor.

let objectMinimumIoU: Float

The value that specifies intersection over union (IOU) that’s the minimum the function treats as an object.

let objectScale: Float

The value that specifies the object confidence loss-scaling factor.

let rescore: Bool

A Boolean value that determines whether to rescore confidence according to prediction verus ground truth Intersection Over Union (IOU).

let whScale: Float

A Boolean value that determines whether to rescore confidence according to prediction verus ground truth Intersection Over Union (IOU).

let xyScale: Float

The value that specifies the x, y loss-scaling factor.

### Initializers

init(huberDelta: Float, gridColumnCount: Int, gridRowsCount: Int, anchorBoxCount: Int, anchorBoxSize: Int, rescore: Bool, xyScale: Float, whScale: Float, objectScale: Float, noObjectScale: Float, classificationScale: Float, objectMinimumIoU: Float, noObjectMaximumIoU: Float, anchorsData: UnsafeMutablePointer&lt;Float>)

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

case yolo(parameters: BNNS.LossFunction.YoloParameters)

You Only Look Once (YOLO) loss computation between prediction and ground truth labels.

Deprecated

