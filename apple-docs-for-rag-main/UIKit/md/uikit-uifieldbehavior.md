

- UIKit
-  UIFieldBehavior 

Class

# UIFieldBehavior

An object that applies field-based physics to dynamic items.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
class UIFieldBehavior
```

## Overview

A field behavior defines an area in which forces such as gravity, magnetism, drag, velocity, turbulence, and others can be applied. After creating a field behavior object of the appropriate type, configure the strength of the intended force along with any other field attributes.

After creating a field behavior object, call the addItem(_:) method to associate the field with that item. For many types of fields, you must also configure a UIDynamicItemBehavior object for the item to define relevant attributes of the item such as its density (mass) or charge. After configuring the field, add it to the UIDynamicAnimator object associated with your interface to begin the animations.

The position of a field defines its location in your interface and the field’s region defines its area of influence. The region you specify is centered on the field’s position. Regions can be circular or rectangular, and you can combine regions in different ways to create more complex region shapes.

Most fields use only a subset of the field attributes in their computations. All fields have a strength value that helps define the intensity of the field. Most fields also use the falloff property to vary the field strength over distance. You configure other attributes only as needed for the type of field.

## Topics

### Getting the field behaviors

class func dragField() -> Self

Creates and returns a field behavior for slowing an object’s velocity.

class func springField() -> Self

Creates and returns a spring field behavior.

class func velocityField(direction: CGVector) -> Self

Creates and returns a field behavior object that applies a directional velocity to items.

class func electricField() -> Self

Creates and returns a field behavior object that interacts with charged items.

class func magneticField() -> Self

Creates and returns a field behavior that interacts with charged items.

class func radialGravityField(position: CGPoint) -> Self

Creates and returns a field behavior object that models a radial gravitational force.

class func linearGravityField(direction: CGVector) -> Self

Creates and returns a field behavior object that models a linear gravitational force.

class func vortexField() -> Self

Creates and returns a field behavior object that applies a rotational force relative to the field’s position.

class func noiseField(smoothness: CGFloat, animationSpeed: CGFloat) -> Self

Creates and returns a field behavior object that applies random noise to other forces.

class func turbulenceField(smoothness: CGFloat, animationSpeed: CGFloat) -> Self

Creates and returns a field behavior object that applies noise to an item in motion.

class func field(evaluationBlock: (UIFieldBehavior, CGPoint, CGVector, CGFloat, CGFloat, TimeInterval) -> CGVector) -> Self

Creates and returns a field behavior object that applies an app-specified field to items.

### Managing the associated dynamic items

func addItem(any UIDynamicItem)

Associates the field behavior with the specified dynamic item.

func removeItem(any UIDynamicItem)

Removes the field behavior from the specified dynamic item.

var items: [any UIDynamicItem]

The dynamic items associated with the current field behavior.

### Configuring the field attributes

var position: CGPoint

The position of the field in the reference coordinate system.

var region: UIRegion

The shape of the field.

var strength: CGFloat

The strength of the field.

var falloff: CGFloat

The rate of decay for the field strength.

var minimumRadius: CGFloat

The minimum distance at which to start calculating new values for the field.

var direction: CGVector

The direction of motion for a linear field.

var smoothness: CGFloat

The smoothness of the noise used to generate the field.

var animationSpeed: CGFloat

The rate at which the animation should proceed.

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

class UIGravityBehavior

An object that applies a gravity-like force to all of its associated dynamic items.

class UIPushBehavior

A behavior that applies a continuous or instantaneous force to one or more dynamic items, causing those items to change position accordingly.

class UISnapBehavior

A spring-like behavior whose initial motion is damped over time so that the object settles at a specific point.

