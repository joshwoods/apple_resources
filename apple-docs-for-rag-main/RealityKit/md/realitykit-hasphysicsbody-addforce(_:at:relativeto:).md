

- RealityKit
- HasPhysicsBody
-  addForce(\_:at:relativeTo:) 

Instance Method

# addForce(\_:at:relativeTo:)

Applies a force to the physics body at the specified position.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func addForce(
    _ force: SIMD3,
    at position: SIMD3,
    relativeTo referenceEntity: Entity?
)
```

## Parameters 

`force`  

A force in newtons.

`position`  

The position at which to apply the force.

`referenceEntity`  

The reference entity that defines the coordinate space in which `position` and `force` are defined.

## Discussion

The physics simulator applies the added force until the end of the frame interval. To continue exerting the force after that time, add the force again with another call to the method. Handle the SceneEvents.Update event to receive an indication of when the frame interval ends. For an app that renders at 60 frames per second (fps), this event occurs about once per 16 milliseconds.

## See Also

### Adding and clearing forces

func addForce(SIMD3&lt;Float>, relativeTo: Entity?)

Applies a force to the physics body at its center of mass.

func addTorque(SIMD3&lt;Float>, relativeTo: Entity?)

Applies a torque to the physics body at its center of mass.

func clearForcesAndTorques()

Clears all forces previously added to the physics body.

