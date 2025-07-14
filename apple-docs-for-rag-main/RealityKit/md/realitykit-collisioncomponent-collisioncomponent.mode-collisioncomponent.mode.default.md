

- RealityKit
- CollisionComponent
- CollisionComponent.Mode
-  CollisionComponent.Mode.default 

Case

# CollisionComponent.Mode.default

A default collision object.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
case `default`
```

## Discussion

When two objects of this type collide, RealityKit computes the full contact details (contact points, normal vectors, penetration depths, and so on) and stores them in the contact set.

Note

Collisions will fall through and do not collide by default, to enable colliding see the CollisionComponent.Mode.colliding mode.

## See Also

### Collision modes

case trigger

A trigger collision object.

