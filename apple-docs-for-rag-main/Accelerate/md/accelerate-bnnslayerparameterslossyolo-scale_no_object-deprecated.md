

- Accelerate
- BNNSLayerParametersLossYolo
-  scale_no_object Deprecated

Instance Property

# scale_no_object

The value that specifies the no-object confidence scaling factor.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
var scale_no_object: Float
```

Deprecated

Use BNNSGraph\* APIs

## See Also

### Instance Properties

var function: BNNSLossFunction

The function that’s used to compute loss.

Deprecated

var i_desc: BNNSNDArrayDescriptor

The descriptor of the input.

Deprecated

var o_desc: BNNSNDArrayDescriptor

The descriptor of the output.

Deprecated

var reduction: BNNSLossReductionFunction

The function that’s used to reduce the computed loss (must be sum reduction for YOLO).

Deprecated

var huber_delta: Float

A value that’s interpreted as width-height loss.

Deprecated

var number_of_grid_columns: Int

The number of columns in the grid.

Deprecated

var number_of_grid_rows: Int

The number of rows in the grid.

Deprecated

var number_of_anchor_boxes: Int

The number of anchor boxes in each cell.

Deprecated

var anchor_box_size: Int

The size of the anchor box.

Deprecated

var rescore: Bool

A Boolean value that determines whether to rescore confidence according to prediction verus ground truth Intersection Over Union (IOU).

Deprecated

var scale_xy: Float

The value that specifies the x, y loss-scaling factor.

Deprecated

var scale_wh: Float

A Boolean value that determines whether to rescore confidence according to prediction verus ground truth Intersection Over Union (IOU).

Deprecated

var scale_object: Float

The value that specifies the object confidence loss-scaling factor.

Deprecated

var object_minimum_iou: Float

The value that specifies intersection over union (IOU) that’s the minimum the function treats as an object.

Deprecated

var no_object_maximum_iou: Float

The value that specifies intersection over union (IOU) that’s the maximum the function treats as not an object.

Deprecated

