

- UIKit
- UIAttachmentBehavior
-  frictionTorque 

Instance Property

# frictionTorque

The amount of force needed to overcome rotational forces around an anchor point.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var frictionTorque: CGFloat { get set }
```

## Discussion

For attachments where each item rotates around an anchor point, use this property to specify the resistance to that rotation. The default value of this property is `0.0`, which causes items to rotate freely with even very small impulses. Higher torque values increase the amount of force needed to cause rotation.

This property has no formal units, so you need to experiment with values to get the behavior that you want.

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

var attachmentRange: UIFloatRange

The range of motion for the attachment behavior.

