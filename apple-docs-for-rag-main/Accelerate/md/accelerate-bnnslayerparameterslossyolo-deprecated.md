

- Accelerate
-  BNNSLayerParametersLossYolo Deprecated

Structure

# BNNSLayerParametersLossYolo

A structure that contains the parameters of a You Only Look Once (YOLO) loss layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
struct BNNSLayerParametersLossYolo
```

Deprecated

Use BNNSGraph\* APIs

## Topics

### Initializers

init(function: BNNSLossFunction, i_desc: BNNSNDArrayDescriptor, o_desc: BNNSNDArrayDescriptor, reduction: BNNSLossReductionFunction, huber_delta: Float, number_of_grid_columns: Int, number_of_grid_rows: Int, number_of_anchor_boxes: Int, anchor_box_size: Int, rescore: Bool, scale_xy: Float, scale_wh: Float, scale_object: Float, scale_no_object: Float, scale_classification: Float, object_minimum_iou: Float, no_object_maximum_iou: Float, anchors_data: UnsafeMutablePointer&lt;Float>)

Returns a new You Only Look Once (YOLO) loss layer parameters structure from the specified parameters.

### Instance Properties

var function: BNNSLossFunction

The function that’s used to compute loss.

var i_desc: BNNSNDArrayDescriptor

The descriptor of the input.

var o_desc: BNNSNDArrayDescriptor

The descriptor of the output.

var reduction: BNNSLossReductionFunction

The function that’s used to reduce the computed loss (must be sum reduction for YOLO).

var huber_delta: Float

A value that’s interpreted as width-height loss.

var number_of_grid_columns: Int

The number of columns in the grid.

var number_of_grid_rows: Int

The number of rows in the grid.

var number_of_anchor_boxes: Int

The number of anchor boxes in each cell.

var anchor_box_size: Int

The size of the anchor box.

var rescore: Bool

A Boolean value that determines whether to rescore confidence according to prediction verus ground truth Intersection Over Union (IOU).

var scale_xy: Float

The value that specifies the x, y loss-scaling factor.

var scale_wh: Float

A Boolean value that determines whether to rescore confidence according to prediction verus ground truth Intersection Over Union (IOU).

var scale_object: Float

The value that specifies the object confidence loss-scaling factor.

var scale_no_object: Float

The value that specifies the no-object confidence scaling factor.

var object_minimum_iou: Float

The value that specifies intersection over union (IOU) that’s the minimum the function treats as an object.

var no_object_maximum_iou: Float

The value that specifies intersection over union (IOU) that’s the maximum the function treats as not an object.

var scale_classification: Float

The value that specifies the classification scaling factor.

var anchors_data: UnsafeMutablePointer&lt;Float>

Maximum IOU for treating as no object.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Loss layers

class LossLayer

A layer object that wraps a loss filter and manages its deinitialization.

Deprecated

struct BNNSLossFunction

Constants that describe loss functions.

struct BNNSLossReductionFunction

Constants that describe reduction functions used by a loss layer.

struct BNNSLayerParametersLossBase

A structure that contains the parameters of a loss layer.

Deprecated

struct BNNSLayerParametersLossHuber

A structure that contains the parameters of a Huber loss layer.

Deprecated

struct BNNSLayerParametersLossSigmoidCrossEntropy

A structure that contains the parameters of a sigmoid cross entropy loss layer.

Deprecated

struct BNNSLayerParametersLossSoftmaxCrossEntropy

A structure that contains the parameters of a softmax cross entropy loss layer.

Deprecated

func BNNSFilterCreateLayerLoss(UnsafeRawPointer, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new loss layer.

Deprecated

func BNNSLossFilterApplyBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeRawPointer, Int, UnsafeRawPointer?, Int, UnsafeMutableRawPointer, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>?, Int) -> Int32

Applies a loss filter to a set of input objects, writing the result to a set of output objects.

Deprecated

func BNNSLossFilterApplyBackwardBatch(BNNSFilter?, Int, UnsafeRawPointer, Int, UnsafeMutablePointer&lt;BNNSNDArrayDescriptor>, Int, UnsafeRawPointer, Int, UnsafeRawPointer?, Int, UnsafePointer&lt;BNNSNDArrayDescriptor>, Int) -> Int32

Applies a loss filter backward to generate gradients.

Deprecated

