

- RealityKit
- CollisionEvents
- CollisionEvents.Began
-  position 

Instance Property

# position

A position representing the estimated point of contact.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
let position: SIMD3
```

## Discussion

The point is an average calculated from the intersecting shapes. It’s specified in the coordinate space of the physics simulation, which means it’s relative to nearestSimulationEntity(for:). If the physics origin is `nil`, the point is given in world space.

## See Also

### Characterizing the collision

let impulse: Float

The total impulse in this collision pair obtained by adding up all the individual impulses applied at each contact point.

