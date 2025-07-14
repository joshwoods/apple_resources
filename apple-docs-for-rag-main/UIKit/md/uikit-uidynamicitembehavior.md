

- UIKit
-  UIDynamicItemBehavior 

Class

# UIDynamicItemBehavior

A base dynamic animation configuration for one or more dynamic items.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UIDynamicItemBehavior
```

## Overview

A *dynamic item* is any iOS or custom object that conforms to the UIDynamicItem protocol. The UIView and UICollectionViewLayoutAttributes classes implement this protocol in iOS 7 and later. You can use a custom object as a dynamic item for such purposes as reacting to rotation or position changes computed by a dynamic animator—an instance of the UIDynamicAnimator class.

One notable and common use of a dynamic item behavior is to confer a velocity to a dynamic item to match the ending velocity of a user gesture.

To use a dynamic item behavior with a dynamic item, perform these two steps:

1.  Associate the item with the behavior using the addItem(_:) method, or initialize a new dynamic item behavior with an array of items using the init(items:) method

2.  Enable the behavior by adding it to an animator using the addBehavior(_:) method

The coordinate system that pertains to a dynamic item behavior, and the types of dynamic items you can use with the behavior, depend on how you initialized the associated animator. For details, see UIDynamicAnimator.

You can disable rotation for a dynamic item behavior’s items by returning false from the allowsRotation property. To configure interaction among the behavior’s items, use the elasticity and friction properties.

You can include a dynamic item behavior in a custom, composite behavior by starting with a UIDynamicBehavior object and adding a dynamic item behavior with the addChildBehavior(_:) method. If you want to influence a dynamic item behavior at each step of a dynamic animation, implement the inherited action method.

If you add more than one dynamic item behavior to an animator, you effectively create a behavior tree. Only one configuration of a given property applies to any given dynamic item. For a property configured in more than one dynamic item behavior, the last one in the behavior tree, starting from the dynamic animator and going depth first toward the dynamic item, wins.

In the case of an animator with exactly one dynamic item behavior, you can restore default values for all dynamic item behavior properties by removing the behavior. In the case of an animator to which you’ve applied multiple dynamic item behaviors, removing one takes its property contribution out of the behavior tree.

## Topics

### Initializing and managing a dynamic item behavior

func addItem(any UIDynamicItem)

Adds a dynamic item to the dynamic item behavior’s item array.

init(items: [any UIDynamicItem])

Initializes a dynamic item behavior with an array of dynamic items.

func removeItem(any UIDynamicItem)

Removes a specific dynamic item from the dynamic item behavior.

var items: [any UIDynamicItem]

Returns the set of dynamic items you’ve added to the dynamic item behavior.

### Configuring a dynamic item behavior

func addAngularVelocity(CGFloat, for: any UIDynamicItem)

Adds a specified angular velocity to a dynamic item.

func addLinearVelocity(CGPoint, for: any UIDynamicItem)

Adds a specified linear velocity to a dynamic item.

var allowsRotation: Bool

Specifies whether rotation is allowed for the behavior’s dynamic items.

var angularResistance: CGFloat

The angular resistance for the behavior’s dynamic items.

func angularVelocity(for: any UIDynamicItem) -> CGFloat

Returns the angular velocity for a specified dynamic item.

func linearVelocity(for: any UIDynamicItem) -> CGPoint

Returns the linear velocity for a specified dynamic item.

var density: CGFloat

The relative mass density of the behavior’s dynamic items.

var elasticity: CGFloat

The amount of elasticity applied to collisions for the behavior’s dynamic items.

var friction: CGFloat

The linear resistance for the behavior’s dynamic items when two slide against each other.

var resistance: CGFloat

The linear resistance for the behavior’s dynamic items, which reduces their linear velocity over time.

var charge: CGFloat

The charge associated with the item.

var isAnchored: Bool

A Boolean value indicating whether the item is anchored to its current position.

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

### Dynamic Items

protocol UIDynamicItem

A set of methods that can make a custom object eligible to participate in UIKit Dynamics.

class UIDynamicItemGroup

A dynamic item that comprises multiple other dynamic items.

