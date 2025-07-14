

- UIKit
-  UIDynamicBehavior 

Class

# UIDynamicBehavior

An object that confers a behavioral configuration on one or more dynamic items, for their participation in 2D animation.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIDynamicBehavior
```

## Overview

A *dynamic item* is any iOS or custom object that conforms to the UIDynamicItem protocol. The UIView and UICollectionViewLayoutAttributes classes implement this protocol starting in iOS 7.0. You can implement this protocol to use a dynamic animator with custom objects for such purposes as reacting to rotation or position changes computed by an animator—an instance of the UIDynamicAnimator class.

This parent class, UIDynamicBehavior, is inherited by the primitive dynamic behavior classes UIAttachmentBehavior, UICollisionBehavior, UIGravityBehavior, UIDynamicItemBehavior, UIPushBehavior, and UISnapBehavior.

You can subclass UIDynamicBehavior. By using the addChildBehavior(_:) method in an instance of this class or in a custom subclass, you can create composite behaviors of your own design.

When you subclass UIDynamicBehavior, you typically need to provide one or more initializers, along with other housekeeping methods such as those implemented in the iOS primitive dynamic behaviors.

To perform per-step logic in a dynamic animation, provide a block object using the action property.

To access the dynamic animator that a dynamic behavior is associated with, use the dynamicAnimator property. To respond to a dynamic behavior being added to or removed from a dynamic animator, implement the willMove(to:) method.

## Topics

### Configuring a dynamic behavior

var action: (() -> Void)?

The block you want to execute during dynamic animation.

func addChildBehavior(UIDynamicBehavior)

Adds a dynamic behavior, as a child, to a custom dynamic behavior.

var childBehaviors: [UIDynamicBehavior]

Returns the array of dynamic behaviors that are children of a custom dynamic behavior.

func removeChildBehavior(UIDynamicBehavior)

Removes a child dynamic behavior from a custom dynamic behavior.

### Responding to changes in the behavior tree

var dynamicAnimator: UIDynamicAnimator?

The dynamic animator that the dynamic behavior is associated with.

func willMove(to: UIDynamicAnimator?)

Called when the dynamic behavior is added to, or removed from, a dynamic animator.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UIAttachmentBehavior
- UICollisionBehavior
- UIDynamicItemBehavior
- UIFieldBehavior
- UIGravityBehavior
- UIPushBehavior
- UISnapBehavior

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Behaviors

class UIAttachmentBehavior

A relationship between two dynamic items, or between a dynamic item and an anchor point.

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

