

- UIKit
-  UICollisionBehaviorDelegate 

Protocol

# UICollisionBehaviorDelegate

To respond to UIKit dynamic item collisions, configure a custom class to adopt the UICollisionBehaviorDelegate protocol. Then, in a collision behavior (an instance of the UICollisionBehavior class), set the delegate to be an instance of your custom class.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
protocol UICollisionBehaviorDelegate : NSObjectProtocol
```

## Overview

The delegate is notified of collisions that occur between the behavior’s dynamic items, or between a dynamic item and a boundary, depending on the behavior’s mode (as set with its collisionMode property). In the case of a collision between an item and the boundary defined by a reference view, the identifier passed to the delegate method is `nil`. (For more on the reference view and the different ways to initialize a dynamic animator, read the Overview in UIDynamicAnimator.)

## Topics

### Responding to UIKit Dynamics collisions

func collisionBehavior(UICollisionBehavior, beganContactFor: any UIDynamicItem, withBoundaryIdentifier: (any NSCopying)?, at: CGPoint)

Called when a collision, between a dynamic item and a collision boundary, has begun.

func collisionBehavior(UICollisionBehavior, beganContactFor: any UIDynamicItem, with: any UIDynamicItem, at: CGPoint)

Called when a collision between two dynamic items has begun.

func collisionBehavior(UICollisionBehavior, endedContactFor: any UIDynamicItem, withBoundaryIdentifier: (any NSCopying)?)

Called when a collision between a dynamic item and a boundary has ended.

func collisionBehavior(UICollisionBehavior, endedContactFor: any UIDynamicItem, with: any UIDynamicItem)

Called when a collision between two dynamic items has ended.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Customizing the collision behavior

var collisionDelegate: (any UICollisionBehaviorDelegate)?

The delegate object that you want to respond to collisions for the collision behavior.

