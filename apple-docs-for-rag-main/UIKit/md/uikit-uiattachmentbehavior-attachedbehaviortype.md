

- UIKit
- UIAttachmentBehavior
-  attachedBehaviorType 

Instance Property

# attachedBehaviorType

The type of the attachment behavior.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var attachedBehaviorType: UIAttachmentBehavior.AttachmentType { get }
```

## Discussion

The available types for attachment behaviors are described in the UIAttachmentBehavior.AttachmentType enum.

## See Also

### Configuring an attachment behavior

var anchorPoint: CGPoint

The anchor point for the attachment behavior, if any.

var damping: CGFloat

The amount of damping to apply to the attachment behavior.

var frequency: CGFloat

The frequency of oscillation for the attachment behavior.

var length: CGFloat

The distance, in points, between the two attachment points of the attachment behavior.

var frictionTorque: CGFloat

The amount of force needed to overcome rotational forces around an anchor point.

var attachmentRange: UIFloatRange

The range of motion for the attachment behavior.

