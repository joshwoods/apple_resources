

- UIKit
- UIAttachmentBehavior
-  attachmentRange 

Instance Property

# attachmentRange

The range of motion for the attachment behavior.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var attachmentRange: UIFloatRange { get set }
```

## Discussion

For sliding attachments, this property defines the range of motion (measured in points) supported along the given axis of translation. The specified range must always contain the value 0, which represents the starting point of movement for items. Items slide along the axis between the minimum and maximum values you specify. Setting this property to zero prevents items from sliding at all along their axis of translation.

For pin attachments, this property defines the amount of rotation (measured in radians) supported in the counter-clockwise and clockwise directions. The specified range must contain the value `0`, which represents the starting angle of each item. Items rotate around the anchor point between the minimum and maximum values you specify. Setting this property to zero prevents items from rotating at all.

The default value of this property is infinite.

## See Also

### Configuring an attachment behavior

var anchorPoint: CGPoint

The anchor point for the attachment behavior, if any.

var attachedBehaviorType: UIAttachmentBehavior.AttachmentType

The type of the attachment behavior.

var damping: CGFloat

The amount of damping to apply to the attachment behavior.

var frequency: CGFloat

The frequency of oscillation for the attachment behavior.

var length: CGFloat

The distance, in points, between the two attachment points of the attachment behavior.

var frictionTorque: CGFloat

The amount of force needed to overcome rotational forces around an anchor point.

