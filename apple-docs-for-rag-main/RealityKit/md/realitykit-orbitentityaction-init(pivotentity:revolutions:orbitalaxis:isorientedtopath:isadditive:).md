

- RealityKit
- OrbitEntityAction
-  init(pivotEntity:revolutions:orbitalAxis:isOrientedToPath:isAdditive:) 

Initializer

# init(pivotEntity:revolutions:orbitalAxis:isOrientedToPath:isAdditive:)

Creates a new orbit entity action.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    pivotEntity: ActionEntityResolution,
    revolutions: Float,
    orbitalAxis: SIMD3 = [0, 1, 0],
    isOrientedToPath: Bool = false,
    isAdditive: Bool = false
)
```

## Parameters 

`pivotEntity`  

The pivot entity that the targeted entity will orbit.

`revolutions`  

The number of rotations to complete before stopping.

`orbitalAxis`  

A vector that describes the axis of rotation (in world space).

`isOrientedToPath`  

Indicates whether the orbiting target entity updates its orientation during the animation to orient itself along the rotation path.

`isAdditive`  

A Boolean value that indicates whether the animation system additively blends the action’s output with the base value.

