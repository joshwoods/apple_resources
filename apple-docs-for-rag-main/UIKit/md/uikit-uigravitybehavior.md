

- UIKit
-  UIGravityBehavior 

Class

# UIGravityBehavior

An object that applies a gravity-like force to all of its associated dynamic items.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIGravityBehavior
```

## Overview

The magnitude and direction of the gravity force are configurable and are applied equally to all associated items. Use this behavior to modify the position of views and other dynamic items in your app’s interface.

You specify the magnitude and direction of the gravity force as a two-dimensional vector in the reference view’s coordinate system. A value of `1.0` imparts the standard UIKit gravity, which corresponds to an acceleration of 1000 points / second² in the direction of the given axis. The default vector in the gravityDirection property is (`0.0`, `1.0`), which causes items to accelerate downward along the positive y axis. If you prefer to set the vector angle and magnitude separately, you can do so using the corresponding properties.

Note

If you want a gravitational force that takes the mass of each object into account, use a UIFieldBehavior object instead. Field behaviors support both linear and radial gravitation fields and take the mass of an object into account, resulting in different amounts of force applied to each object.

If you want to influence a gravity behavior at each step of a dynamic animation, assign an appropriate block to the inherited action property. Use your block to make any needed changes to the dynamic items associated with the gravity behavior.

### Applying a Gravity Behavior to an Item

To apply a gravity behavior to one or more dynamic items, do the following:

1.  Initialize the behavior using the init(items:) method, passing in the items you want associated with the behavior. Use the addItem(_:) method to add items after initialization. For more information about dynamic items, see UIDynamicItem.

2.  Enable the gravity behavior by adding it to your UIDynamicAnimator object using the addBehavior(_:) method. (Do not add more than one gravity behavior to an animator.)

The gravity behavior derives its coordinate system from the reference view of its associated dynamic animator object. For more information about the dynamic animator and the reference coordinate system, see UIDynamicAnimator.

## Topics

### Initializing a gravity behavior

init(items: [any UIDynamicItem])

Initializes a gravity behavior with an array of dynamic items.

### Managing a gravity behavior’s items

var items: [any UIDynamicItem]

The set of dynamic items associated with the gravity behavior.

func addItem(any UIDynamicItem)

Associates the specified dynamic item with the gravity behavior.

func removeItem(any UIDynamicItem)

Removes the specified dynamic item from the gravity behavior.

### Configuring a gravity behavior

var gravityDirection: CGVector

The direction and magnitude of the gravitational force, expressed as a vector.

var angle: CGFloat

The direction of the gravity vector, expressed in radians in the reference coordinate system.

var magnitude: CGFloat

The magnitude of the gravity vector.

func setAngle(CGFloat, magnitude: CGFloat)

Sets the angle and magnitude of the gravity vector for the behavior.

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

class UIPushBehavior

A behavior that applies a continuous or instantaneous force to one or more dynamic items, causing those items to change position accordingly.

class UISnapBehavior

A spring-like behavior whose initial motion is damped over time so that the object settles at a specific point.

