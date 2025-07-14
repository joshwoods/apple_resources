

- UIKit
- UICollisionBehaviorDelegate
-  collisionBehavior(\_:endedContactFor:withBoundaryIdentifier:) 

Instance Method

# collisionBehavior(\_:endedContactFor:withBoundaryIdentifier:)

Called when a collision between a dynamic item and a boundary has ended.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func collisionBehavior(
    _ behavior: UICollisionBehavior,
    endedContactFor item: any UIDynamicItem,
    withBoundaryIdentifier identifier: (any NSCopying)?
)
```

## Parameters 

`behavior`  

The collision behavior that owns the dynamic item that has ended contact.

`item`  

The dynamic item that collided.

`identifier`  

The identifier of the boundary that the dynamic item collided with.

## See Also

### Responding to UIKit Dynamics collisions

func collisionBehavior(UICollisionBehavior, beganContactFor: any UIDynamicItem, withBoundaryIdentifier: (any NSCopying)?, at: CGPoint)

Called when a collision, between a dynamic item and a collision boundary, has begun.

func collisionBehavior(UICollisionBehavior, beganContactFor: any UIDynamicItem, with: any UIDynamicItem, at: CGPoint)

Called when a collision between two dynamic items has begun.

func collisionBehavior(UICollisionBehavior, endedContactFor: any UIDynamicItem, with: any UIDynamicItem)

Called when a collision between two dynamic items has ended.

