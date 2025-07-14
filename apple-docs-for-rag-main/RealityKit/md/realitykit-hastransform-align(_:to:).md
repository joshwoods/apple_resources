

- RealityKit
- HasTransform
-  align(\_:to:) 

Instance Method

# align(\_:to:)

Moves and rotates the entity by a transformation from the origin pin to the target pin.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@discardableResult @MainActor @preconcurrency
func align(
    _ originPin: GeometricPin,
    to targetPin: GeometricPin
) -> float4x4?
```

## Parameters 

`originPin`  

The `GeometricPin` to align. It should be one of the pins on the entity.

`targetPin`  

The `GeometricPin` to align to.

## Return Value

Transformation matrix that has been applied to the `Entity`, in the frame or reference of the parent of the `Entity`. If either pin doesn’t exist, returns `nil`.

## See Also

### Moving an entity

func move(to: Transform, relativeTo: Entity?)

Moves an entity instantly to a new location given by a transform.

func move(to: float4x4, relativeTo: Entity?)

Moves an entity instantly to a new location given by a 4x4 matrix.

func look(at: SIMD3&lt;Float>, from: SIMD3&lt;Float>, upVector: SIMD3&lt;Float>, relativeTo: Entity?)

Positions and orients the entity to look at a target from a given position.

func look(at: SIMD3&lt;Float>, from: SIMD3&lt;Float>, upVector: SIMD3&lt;Float>, relativeTo: Entity?, forward: Entity.ForwardDirection)

Positions and orients the entity such that it looks at certain target from a give position.

