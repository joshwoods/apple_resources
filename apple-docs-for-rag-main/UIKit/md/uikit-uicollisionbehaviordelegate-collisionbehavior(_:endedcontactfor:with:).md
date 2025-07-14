

- UIKit
- UICollisionBehaviorDelegate
-  collisionBehavior(\_:endedContactFor:with:) 

Instance Method

# collisionBehavior(\_:endedContactFor:with:)

Called when a collision between two dynamic items has ended.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func collisionBehavior(
    _ behavior: UICollisionBehavior,
    endedContactFor item1: any UIDynamicItem,
    with item2: any UIDynamicItem
)
```

## Parameters 

`behavior`  

The collision behavior that owns the dynamic items that collided.

`item1`  

The first of the two dynamic items participating in the collision.

`item2`  

The second of the two dynamic items participating in the collision.

## See Also

### Responding to UIKit Dynamics collisions

func collisionBehavior(UICollisionBehavior, beganContactFor: any UIDynamicItem, withBoundaryIdentifier: (any NSCopying)?, at: CGPoint)

Called when a collision, between a dynamic item and a collision boundary, has begun.

func collisionBehavior(UICollisionBehavior, beganContactFor: any UIDynamicItem, with: any UIDynamicItem, at: CGPoint)

Called when a collision between two dynamic items has begun.

func collisionBehavior(UICollisionBehavior, endedContactFor: any UIDynamicItem, withBoundaryIdentifier: (any NSCopying)?)

Called when a collision between a dynamic item and a boundary has ended.

