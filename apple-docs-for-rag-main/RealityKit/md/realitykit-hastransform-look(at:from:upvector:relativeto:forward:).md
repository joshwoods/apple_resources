

- RealityKit
- HasTransform
-  look(at:from:upVector:relativeTo:forward:) 

Instance Method

# look(at:from:upVector:relativeTo:forward:)

Positions and orients the entity such that it looks at certain target from a give position.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
func look(
    at target: SIMD3,
    from position: SIMD3,
    upVector: SIMD3 = SIMD3(0, 1, 0),
    relativeTo referenceEntity: Entity?,
    forward: Entity.ForwardDirection = .negativeZ
)
```

## Parameters 

`target`  

The target position to look at.

`position`  

The new position of the entity.

`upVector`  

The *up* direction of the entity.

`referenceEntity`  

The reference entity which defines the frame of reference. Can be `nil`, which is equivalent to “world space”.

`forward`  

Use default forward (.negativeZ). Can be set to .positiveZ for non-camera entities

## Discussion

This function moves the entity to the specified `position`. It rotates the entity such that the forward direction is pointing towards `target`. It further makes sure that entity’s *up* direction aligns with the specified `upVector`.

Note

This method can be used for non-camera entities.

## See Also

### Moving an entity

func move(to: Transform, relativeTo: Entity?)

Moves an entity instantly to a new location given by a transform.

func move(to: float4x4, relativeTo: Entity?)

Moves an entity instantly to a new location given by a 4x4 matrix.

func look(at: SIMD3&lt;Float>, from: SIMD3&lt;Float>, upVector: SIMD3&lt;Float>, relativeTo: Entity?)

Positions and orients the entity to look at a target from a given position.

func align(GeometricPin, to: GeometricPin) -> float4x4?

Moves and rotates the entity by a transformation from the origin pin to the target pin.

