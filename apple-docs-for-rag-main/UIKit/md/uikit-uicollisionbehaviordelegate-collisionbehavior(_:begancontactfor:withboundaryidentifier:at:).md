

- UIKit
- UICollisionBehaviorDelegate
-  collisionBehavior(\_:beganContactFor:withBoundaryIdentifier:at:) 

Instance Method

# collisionBehavior(\_:beganContactFor:withBoundaryIdentifier:at:)

Called when a collision, between a dynamic item and a collision boundary, has begun.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func collisionBehavior(
    _ behavior: UICollisionBehavior,
    beganContactFor item: any UIDynamicItem,
    withBoundaryIdentifier identifier: (any NSCopying)?,
    at p: CGPoint
)
```

## Parameters 

`behavior`  

The collision behavior that owns the dynamic item that has started contact with a boundary.

`item`  

The dynamic item that has started contact with a boundary.

`identifier`  

The identifier of the boundary that the dynamic item has started contact with.

`p`  

The collision point on the boundary.

## See Also

### Responding to UIKit Dynamics collisions

func collisionBehavior(UICollisionBehavior, beganContactFor: any UIDynamicItem, with: any UIDynamicItem, at: CGPoint)

Called when a collision between two dynamic items has begun.

func collisionBehavior(UICollisionBehavior, endedContactFor: any UIDynamicItem, withBoundaryIdentifier: (any NSCopying)?)

Called when a collision between a dynamic item and a boundary has ended.

func collisionBehavior(UICollisionBehavior, endedContactFor: any UIDynamicItem, with: any UIDynamicItem)

Called when a collision between two dynamic items has ended.

