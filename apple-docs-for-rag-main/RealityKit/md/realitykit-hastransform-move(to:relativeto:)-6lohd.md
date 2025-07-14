

- RealityKit
- HasTransform
-  move(to:relativeTo:) 

Instance Method

# move(to:relativeTo:)

Moves an entity instantly to a new location given by a transform.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func move(
    to transform: Transform,
    relativeTo referenceEntity: Entity?
)
```

## Parameters 

`transform`  

A Transform instance that indicates the new location.

`referenceEntity`  

The entity that defines a frame of reference. Set this to `nil` to indicate world space.

## See Also

### Moving an entity

func move(to: float4x4, relativeTo: Entity?)

Moves an entity instantly to a new location given by a 4x4 matrix.

func look(at: SIMD3&lt;Float>, from: SIMD3&lt;Float>, upVector: SIMD3&lt;Float>, relativeTo: Entity?)

Positions and orients the entity to look at a target from a given position.

func look(at: SIMD3&lt;Float>, from: SIMD3&lt;Float>, upVector: SIMD3&lt;Float>, relativeTo: Entity?, forward: Entity.ForwardDirection)

Positions and orients the entity such that it looks at certain target from a give position.

func align(GeometricPin, to: GeometricPin) -> float4x4?

Moves and rotates the entity by a transformation from the origin pin to the target pin.

