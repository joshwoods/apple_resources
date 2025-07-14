

- RealityKit
- CollisionGroup
-  default 

Type Property

# default

The default collision group for objects.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
static let `default`: CollisionGroup
```

## Discussion

If no CollisionFilter is assigned to an entity, that entity will be part of this default collision group.

## See Also

### Standard collision groups

static let all: CollisionGroup

The collision group that represents all groups.

static let sceneUnderstanding: CollisionGroup

The default collision group for scene-understanding meshes.

