

- UIKit
-  UISnapBehavior 

Class

# UISnapBehavior

A spring-like behavior whose initial motion is damped over time so that the object settles at a specific point.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UISnapBehavior
```

## Overview

A **dynamic item** is any iOS or custom object that conforms to the UIDynamicItem protocol. The UIView and UICollectionViewLayoutAttributes classes implement this protocol starting in iOS 7.0. You can use a custom object as a dynamic item for such purposes as reacting to rotation or position changes computed by a dynamic animator—an instance of the UIDynamicAnimator class.

To use a snap behavior with a dynamic item, perform these two steps:

1.  Initialize a new snap behavior with the item using the init(item:snapTo:) method

2.  Enable the behavior by adding it to an animator using the addBehavior(_:) method

The coordinate system that pertains to a snap behavior, and the types of dynamic items you can use with the behavior, depend on how you initialized the associated animator. For details, read the Overview of UIDynamicAnimator.

You can include a snap behavior in a custom, composite behavior by starting with a UIDynamicBehavior object and adding a snap behavior with the addChildBehavior(_:) method. If you want to influence a snap behavior at each step of a dynamic animation, implement the inherited action method.

## Topics

### Initializing a snap behavior

init(item: any UIDynamicItem, snapTo: CGPoint)

Initializes a snap behavior with a dynamic item and a snap point.

### Configuring a snap behavior

var snapPoint: CGPoint

The point to which to snap.

var damping: CGFloat

The amount of oscillation of a dynamic item during the conclusion of a snap.

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
- Sendable

## See Also

### Behaviors

class UIDynamicBehavior

An object that confers a behavioral configuration on one or more dynamic items, for their participation in 2D animation.

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

