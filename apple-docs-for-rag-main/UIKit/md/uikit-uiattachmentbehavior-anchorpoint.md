

- UIKit
- UIAttachmentBehavior
-  anchorPoint 

Instance Property

# anchorPoint

The anchor point for the attachment behavior, if any.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var anchorPoint: CGPoint { get set }
```

## Discussion

The anchor point is relative to the coordinate system for the behavior’s associated dynamic animator. For attachment types without an anchor point, the value in this property is CGPointZero. For more information about the coordinate system of the reference view, see UIDynamicAnimator.

## See Also

### Configuring an attachment behavior

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

var attachmentRange: UIFloatRange

The range of motion for the attachment behavior.

