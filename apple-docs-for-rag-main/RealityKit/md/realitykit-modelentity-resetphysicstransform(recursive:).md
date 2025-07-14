

- RealityKit
- ModelEntity
-  resetPhysicsTransform(recursive:) 

Instance Method

# resetPhysicsTransform(recursive:)

Resets the position, orientation, and velocities of the simulated physics body.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func resetPhysicsTransform(recursive: Bool = true)
```

## Parameters 

`recursive`  

Apply the reset to all descendant entities.

## Discussion

Call this method only for dynamic rigid bodies, with a mode of PhysicsBodyMode.dynamic. This is the only kind of body that’s affected by physics simulations. For all others, modify the entity’s transform property directly.

Conversely, directly modifying the transform of a dynamic body has no effect because the physics simulation overwrites it on every frame.

## See Also

### Simulating forces, impulses, and motion

var physicsBody: PhysicsBodyComponent?

A component that is used for physics simulations of the model entity in accordance with the laws of Newtonian mechanics.

var physicsMotion: PhysicsMotionComponent?

The physics motion component used by physics simulations of the model entity.

func addForce(SIMD3&lt;Float>, relativeTo: Entity?)

Applies a force to the physics body at its center of mass.

func addForce(SIMD3&lt;Float>, at: SIMD3&lt;Float>, relativeTo: Entity?)

Applies a force to the physics body at the specified position.

func addTorque(SIMD3&lt;Float>, relativeTo: Entity?)

Applies a torque to the physics body at its center of mass.

func clearForcesAndTorques()

Clears all forces previously added to the physics body.

func applyLinearImpulse(SIMD3&lt;Float>, relativeTo: Entity?)

Applies an impulse to the physics body at its center of mass.

func applyAngularImpulse(SIMD3&lt;Float>, relativeTo: Entity?)

Applies an angular (torque) impulse to the physics body at its center of mass.

func applyImpulse(SIMD3&lt;Float>, at: SIMD3&lt;Float>, relativeTo: Entity?)

Applies an impulse to the physics body at the specified position.

func resetPhysicsTransform(Transform, recursive: Bool)

Resets the position and velocities of the simulated physics body.

Deprecated

