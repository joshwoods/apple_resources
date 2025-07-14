

- UIKit
-  UICollisionBehavior 

Class

# UICollisionBehavior

An object that confers to a specified array of dynamic items the ability to engage in collisions with each other and with the behavior’s specified boundaries.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UICollisionBehavior
```

## Overview

A collision behavior also specifies some characteristics of its items’ collisions, with other characteristics optionally specified by a UIDynamicItemBehavior object. A *dynamic item* is any iOS or custom object that conforms to the UIDynamicItem protocol. The UIView and UICollectionViewLayoutAttributes classes implement this protocol starting in iOS 7.0. You can use a custom object as a dynamic item for such purposes as reacting to rotation or position changes computed by a dynamic animator—an instance of the UIDynamicAnimator class.

To use a collision behavior with a dynamic item, perform these two steps:

1.  Associate the item with the behavior using the addItem(_:) method, or initialize a new collision behavior with an array of items using the init(items:) method.

2.  Enable the behavior by adding it to an animator using the addBehavior(_:) method

The coordinate system that pertains to a collision behavior, and the types of dynamic items you can use with the behavior, depend on how you initialized the associated animator. For details, read the Overview of UIDynamicAnimator.

You can add multiple collision behaviors to a dynamic animator. A dynamic item can be part of any number of collision behaviors, provided those behaviors belong to the same animator. For example, you can specify a collision behavior for a set of say, blue, items and another for, say, pink items. When you add both behaviors to a dynamic animator, blue items can collide with each other and pink items can collide with each other, but a blue item and a pink item would not collide—they would ignore each other.

By default, a collision behavior’s items can collide with each other *and* with any boundaries you’ve specified for the behavior. If you want to specify that a behavior’s items collide only with each other, or only with boundaries, explicitly set the collisionMode property.

You can define a collision boundary with a bezier path (see the addBoundary(withIdentifier:for:) method) or with a line segment (see the addBoundary(withIdentifier:from:to:) method). When you use a collision behavior with a dynamic animator you’ve initialized with a reference view or a collection view layout, you can also specify a collision boundary according to the bounds of the dynamic animator’s coordinate system (see the setTranslatesReferenceBoundsIntoBoundary(with:) method).

Important

When setting the initial position for a dynamic item, you must ensure that its bounds do not intersect any collision boundaries. The animation behavior for such a misplaced item is undefined.

To respond to collisions, implement a delegate object that adopts the UICollisionBehaviorDelegate protocol. Add the delegate to the behavior using the collisionDelegate property.

You can include a collision behavior in a custom, composite behavior by starting with a UIDynamicBehavior object and adding a collision behavior with the addChildBehavior(_:) method. If you want to influence a collision behavior at each step of a dynamic animation, implement the inherited action method.

## Topics

### Initializing and managing a collision behavior

func addItem(any UIDynamicItem)

Adds a dynamic item to the collision behavior’s item array.

init(items: [any UIDynamicItem])

Initializes a collision behavior with an array of dynamic items.

func removeItem(any UIDynamicItem)

Removes a specific dynamic item from the collision behavior.

var items: [any UIDynamicItem]

Returns the set of dynamic items you’ve added to the collision behavior.

### Customizing the collision behavior

var collisionDelegate: (any UICollisionBehaviorDelegate)?

The delegate object that you want to respond to collisions for the collision behavior.

protocol UICollisionBehaviorDelegate

To respond to UIKit dynamic item collisions, configure a custom class to adopt the UICollisionBehaviorDelegate protocol. Then, in a collision behavior (an instance of the UICollisionBehavior class), set the delegate to be an instance of your custom class.

### Configuring a collision behavior

func addBoundary(withIdentifier: any NSCopying, for: UIBezierPath)

Adds a collision boundary, specified as a Bezier path, to the collision behavior.

func addBoundary(withIdentifier: any NSCopying, from: CGPoint, to: CGPoint)

Adds a collision boundary, specified as a line segment, to the collision behavior.

var boundaryIdentifiers: [any NSCopying]?

The set of boundary identifiers that you’ve added to the collision behavior.

func boundary(withIdentifier: any NSCopying) -> UIBezierPath?

Returns a specified Bezier-path boundary.

var collisionMode: UICollisionBehavior.Mode

The type of edges that participate in collisions for the collision behavior.

func removeAllBoundaries()

Removes all previously-specified collision boundaries from the collision behavior.

func removeBoundary(withIdentifier: any NSCopying)

Removes a specific collision boundary from the collision behavior.

func setTranslatesReferenceBoundsIntoBoundary(with: UIEdgeInsets)

Specifies a collision boundary based on the bounds of the animation reference system, with optional insets.

var translatesReferenceBoundsIntoBoundary: Bool

Specifies whether a boundary based on the reference system is active.

### Constants

struct Mode

The types of edges that participate in collisions for a collision behavior.

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

class UIFieldBehavior

An object that applies field-based physics to dynamic items.

class UIGravityBehavior

An object that applies a gravity-like force to all of its associated dynamic items.

class UIPushBehavior

A behavior that applies a continuous or instantaneous force to one or more dynamic items, causing those items to change position accordingly.

class UISnapBehavior

A spring-like behavior whose initial motion is damped over time so that the object settles at a specific point.

