

- RealityKit
- HasTransform
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

## See Also

### Moving an entity

func move(to: Transform, relativeTo: Entity?)

Moves an entity instantly to a new location given by a transform.

func move(to: float4x4, relativeTo: Entity?)

Moves an entity instantly to a new location given by a 4x4 matrix.

func look(at: SIMD3&lt;Float>, from: SIMD3&lt;Float>, upVector: SIMD3&lt;Float>, relativeTo: Entity?, forward: Entity.ForwardDirection)

Positions and orients the entity such that it looks at certain target from a give position.

func align(GeometricPin, to: GeometricPin) -> float4x4?

Moves and rotates the entity by a transformation from the origin pin to the target pin.

