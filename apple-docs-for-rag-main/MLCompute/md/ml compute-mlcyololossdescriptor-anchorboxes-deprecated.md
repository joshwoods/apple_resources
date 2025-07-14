

- ML Compute
- MLCYOLOLossDescriptor
-  anchorBoxes Deprecated

Instance Property

# anchorBoxes

Data that contains the width and height for all the anchor boxes.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
var anchorBoxes: Data { get }
```

## Discussion

This data has anchorBoxCount pairs of floating-point values that represent the width and height of each anchor box.

## See Also

### Inspecting YOLO Loss Descriptors

var anchorBoxCount: Int

The number of anchor boxes you use to detect an object in each grid cell.

Deprecated

var maximumIOUForObjectAbsence: Float

The negative intersection over union (IOU).

Deprecated

var minimumIOUForObjectPresence: Float

The positive intersection over union (IOU).

Deprecated

var scaleClassLoss: Float

The scale factor you use for loss when there are no object classes, and for loss gradient.

Deprecated

var scaleObjectConfidenceLoss: Float

The scale factor you use for object confidence loss and loss gradient.

Deprecated

var scaleNoObjectConfidenceLoss: Float

The scale factor you use for no object confidence loss and loss gradient.

Deprecated

var scaleSpatialPositionLoss: Float

The scale factor you use for spatial position loss and loss gradient.

Deprecated

var scaleSpatialSizeLoss: Float

The scale factor you use for spatial size loss and loss gradient.

Deprecated

var shouldRescore: Bool

A Boolean that indicates whether the layer scales the object confidence loss by the intersection over union (IOU) overlap.

Deprecated

