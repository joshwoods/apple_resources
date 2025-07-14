

- UIKit
- UICollisionBehaviorDelegate
-  collisionBehavior(\_:beganContactFor:with:at:) 

Instance Method

# collisionBehavior(\_:beganContactFor:with:at:)

Called when a collision between two dynamic items has begun.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func collisionBehavior(
    _ behavior: UICollisionBehavior,
    beganContactFor item1: any UIDynamicItem,
    with item2: any UIDynamicItem,
    at p: CGPoint
)
```

## Parameters 

`behavior`  

The collision behavior that owns the dynamic items that have started to contact each other.

`item1`  

The first of the two dynamic items participating in the collision.

`item2`  

The second of the two dynamic items participating in the collision.

`p`  

The contact point for the collision. The coordinate system that pertains to a collision depends on how you initialized the associated animator. For details, read the Overview of UIDynamicAnimator.

## See Also

### Responding to UIKit Dynamics collisions

func collisionBehavior(UICollisionBehavior, beganContactFor: any UIDynamicItem, withBoundaryIdentifier: (any NSCopying)?, at: CGPoint)

Called when a collision, between a dynamic item and a collision boundary, has begun.

func collisionBehavior(UICollisionBehavior, endedContactFor: any UIDynamicItem, withBoundaryIdentifier: (any NSCopying)?)

Called when a collision between a dynamic item and a boundary has ended.

func collisionBehavior(UICollisionBehavior, endedContactFor: any UIDynamicItem, with: any UIDynamicItem)

Called when a collision between two dynamic items has ended.

