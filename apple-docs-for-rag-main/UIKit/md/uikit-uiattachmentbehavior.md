

- UIKit
-  UIAttachmentBehavior 

Class

# UIAttachmentBehavior

A relationship between two dynamic items, or between a dynamic item and an anchor point.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIAttachmentBehavior
```

## Overview

When two items are attached to each other, forces imparted on one item affect the movement of the other in a prescribed way. When an item is attached to an anchor point, the movement of that item is affected by its attachment to the specified anchor point. Some attachment behaviors support both two items and an anchor point.

You specify type of attachment behavior you want at creation time. This class offers many creation and initialization methods, each of which creates a different type of attachment behavior, which cannot be changed later. However, you may change specific attributes of the attachment behavior using the properties of this class. For example, you can change the distance between two attached items or change the damping forces applied to the items.

### Applying an Attachment Behavior to Dynamic Items

To apply an attachment behavior to your dynamic items, do the following:

1.  Create the attachment behavior using one of the creation or initialization methods. The method you choose defines the relationship between the items and the anchor point (if any).

2.  Enable the attachment behavior by adding it to your UIDynamicAnimator object using the addBehavior(_:) method. Do not add the same attachment behavior to multiple animator objects.

The attachment behavior derives its coordinate system from the reference view of its associated dynamic animator object. For more information about the dynamic animator and the reference coordinate system, see UIDynamicAnimator.

## Topics

### Creating and initializing attachment behavior objects

class func slidingAttachment(with: any UIDynamicItem, attachmentAnchor: CGPoint, axisOfTranslation: CGVector) -> Self

Creates and returns an attachment behavior where one item slides along the specified axis.

class func slidingAttachment(with: any UIDynamicItem, attachedTo: any UIDynamicItem, attachmentAnchor: CGPoint, axisOfTranslation: CGVector) -> Self

Creates and returns an attachment behavior where two items are fixed to points that slide along the specified axis.

class func fixedAttachment(with: any UIDynamicItem, attachedTo: any UIDynamicItem, attachmentAnchor: CGPoint) -> Self

Creates and returns an attachment behavior where the two items are fixed together through the specified anchor point.

class func limitAttachment(with: any UIDynamicItem, offsetFromCenter: UIOffset, attachedTo: any UIDynamicItem, offsetFromCenter: UIOffset) -> Self

Creates and returns an attachment behavior object where two items are constrained by a maximum distance from one another.

class func pinAttachment(with: any UIDynamicItem, attachedTo: any UIDynamicItem, attachmentAnchor: CGPoint) -> Self

Creates and returns an attachment behavior where the two items are pinned to, and move around, an anchor point

convenience init(item: any UIDynamicItem, attachedToAnchor: CGPoint)

Initializes a behavior where the center of a dynamic item is attached to the specified anchor point.

convenience init(item: any UIDynamicItem, attachedTo: any UIDynamicItem)

Initializes a behavior where the centers of two dynamic items are attached to each other.

init(item: any UIDynamicItem, offsetFromCenter: UIOffset, attachedToAnchor: CGPoint)

Initializes a behavior where the specified point in a dynamic item is attached to an anchor point.

init(item: any UIDynamicItem, offsetFromCenter: UIOffset, attachedTo: any UIDynamicItem, offsetFromCenter: UIOffset)

Initializes an attachment behavior that connects a specified point in one dynamic item to a specified point in another dynamic item.

### Getting the attached items

var items: [any UIDynamicItem]

The dynamic items connected by the attachment behavior.

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

var attachmentRange: UIFloatRange

The range of motion for the attachment behavior.

### Constants

enum AttachmentType

Constants indicating the type of the attachment behavior object.

struct UIFloatRange

The range of motion for attached objects.

Float range constants

Constants for specifying standard ranges.

struct UIOffset

A structure that specifies an amount to offset a position.

## Relationships

### Inherits From

- UIDynamicBehavior

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Behaviors

class UIDynamicBehavior

An object that confers a behavioral configuration on one or more dynamic items, for their participation in 2D animation.

class UICollisionBehavior

An object that confers to a specified array of dynamic items the ability to engage in collisions with each other and with the behavior’s specified boundaries.

class UIFieldBehavior

An object that applies field-based physics to dynamic items.

class UIGravityBehavior

An object that applies a gravity-like force to all of its associated dynamic items.

class UIPushBehavior

A behavior that applies a continuous or instantaneous force to one or more dynamic items, causing those items to change position accordingly.

class UISnapBehavior

A spring-like behavior whose initial motion is damped over time so that the object settles at a specific point.

