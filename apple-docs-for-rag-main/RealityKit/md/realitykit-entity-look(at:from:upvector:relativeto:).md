

- RealityKit
- Entity
-  look(at:from:upVector:relativeTo:) 

Instance Method

# look(at:from:upVector:relativeTo:)

Positions and orients the entity to look at a target from a given position.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func look(
    at target: SIMD3,
    from position: SIMD3,
    upVector: SIMD3 = SIMD3(0, 1, 0),
    relativeTo referenceEntity: Entity?
)
```

## Parameters 

`target`  

The target position to look at.

`position`  

The new position of the entity.

`upVector`  

The up direction of the entity after moving.

`referenceEntity`  

The entity that defines a frame of reference. Set this to `nil` to indicate world space.

## Discussion

You can use this method on any entity, but it’s particularly useful for orienting cameras and lights to aim at a particular point in space.

