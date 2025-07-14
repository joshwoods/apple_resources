

- UIKit
- UIAttachmentBehavior
-  length 

Instance Property

# length

The distance, in points, between the two attachment points of the attachment behavior.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var length: CGFloat { get set }
```

## Discussion

Use this property to adjust the attachment length, if you want to, *after* creating an attachment. The system sets initial length automatically based on how you initialize the attachment.

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

var frictionTorque: CGFloat

The amount of force needed to overcome rotational forces around an anchor point.

var attachmentRange: UIFloatRange

The range of motion for the attachment behavior.

