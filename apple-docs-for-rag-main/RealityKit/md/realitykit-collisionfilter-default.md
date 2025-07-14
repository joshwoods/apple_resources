

- RealityKit
- CollisionFilter
-  default 

Type Property

# default

The default collision filter.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
static let `default`: CollisionFilter
```

## Discussion

Entities with a default collision filter have a group of default and a mask of all.

## See Also

### Creating a collision filter

init(group: CollisionGroup, mask: CollisionGroup)

Creates a collision filter.

static let sensor: CollisionFilter

A collision filter for an entity that collides with everything.

