

- RealityKit
- CollisionComponent
- CollisionComponent.Mode
-  CollisionComponent.Mode.trigger 

Case

# CollisionComponent.Mode.trigger

A trigger collision object.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
case trigger
```

## Discussion

When a collision object of this type collides with any other object, RealityKit records that contact was made, but does not compute other details, like contact points, normal vectors, and so on. This makes a trigger object more performant when all you need is a Boolean indicator that contact occurred.

Triggers are not simulated, so if the Entity also contains PhysicsBodyComponent, `trigger` is ignored.

## See Also

### Collision modes

case `default`

A default collision object.

