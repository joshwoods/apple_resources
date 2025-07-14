

- RealityKit
- CollisionFilter
-  sensor 

Type Property

# sensor

A collision filter for an entity that collides with everything.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
static let sensor: CollisionFilter
```

## Discussion

The sensor collision filter is typically used by rays in ray casts, shapes in convex shape casts, and trigger volumes. It corresponds to a group and mask both set to all.

## See Also

### Creating a collision filter

init(group: CollisionGroup, mask: CollisionGroup)

Creates a collision filter.

static let `default`: CollisionFilter

The default collision filter.

