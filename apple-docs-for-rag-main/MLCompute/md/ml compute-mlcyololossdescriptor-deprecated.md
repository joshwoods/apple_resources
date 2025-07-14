

- ML Compute
-  MLCYOLOLossDescriptor Deprecated

Class

# MLCYOLOLossDescriptor

The configuration object you use to create the YOLO loss layer.

iOS 14.0–17.4DeprecatediPadOS 14.0–17.4DeprecatedMac Catalyst 14.0–17.4DeprecatedmacOS 11.0–14.3DeprecatedtvOS 14.0–17.4Deprecated

``` source
class MLCYOLOLossDescriptor
```

## Topics

### Creating YOLO Loss Descriptors

convenience init(anchorBoxes: Data, anchorBoxCount: Int)

Creates a YOLO loss filter descriptor with the anchor box data and number of anchor boxes you specify.

### Inspecting YOLO Loss Descriptors

var anchorBoxCount: Int

The number of anchor boxes you use to detect an object in each grid cell.

var anchorBoxes: Data

Data that contains the width and height for all the anchor boxes.

var maximumIOUForObjectAbsence: Float

The negative intersection over union (IOU).

var minimumIOUForObjectPresence: Float

The positive intersection over union (IOU).

var scaleClassLoss: Float

The scale factor you use for loss when there are no object classes, and for loss gradient.

var scaleObjectConfidenceLoss: Float

The scale factor you use for object confidence loss and loss gradient.

var scaleNoObjectConfidenceLoss: Float

The scale factor you use for no object confidence loss and loss gradient.

var scaleSpatialPositionLoss: Float

The scale factor you use for spatial position loss and loss gradient.

var scaleSpatialSizeLoss: Float

The scale factor you use for spatial size loss and loss gradient.

var shouldRescore: Bool

A Boolean that indicates whether the layer scales the object confidence loss by the intersection over union (IOU) overlap.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Creating YOLO Loss Layers

convenience init(descriptor: MLCYOLOLossDescriptor)

Creates a YOLO loss layer with the descriptor you specify.

Deprecated

