

- RealityKit
- ModelEntity
-  addForce(\_:relativeTo:) 

Instance Method

# addForce(\_:relativeTo:)

Applies a force to the physics body at its center of mass.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func addForce(
    _ force: SIMD3,
    relativeTo referenceEntity: Entity?
)
```

## Parameters 

`force`  

A force in newtons.

`referenceEntity`  

The reference entity that defines the coordinate space in which `force` is defined.

## Mentioned in 

Manipulating Reality Composer scenes from code

## Discussion

The physics simulator applies the added force until the end of the frame interval. To continue exerting the force after that time, add the force again with another call to the method. Handle the SceneEvents.Update event to receive an indication of when the frame interval ends. For an app that renders at 60 frames per second (fps), this event occurs about once per 16 milliseconds.

## See Also

### Simulating forces, impulses, and motion

var physicsBody: PhysicsBodyComponent?

A component that is used for physics simulations of the model entity in accordance with the laws of Newtonian mechanics.

var physicsMotion: PhysicsMotionComponent?

The physics motion component used by physics simulations of the model entity.

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

func resetPhysicsTransform(recursive: Bool)

Resets the position, orientation, and velocities of the simulated physics body.

func resetPhysicsTransform(Transform, recursive: Bool)

Resets the position and velocities of the simulated physics body.

Deprecated

