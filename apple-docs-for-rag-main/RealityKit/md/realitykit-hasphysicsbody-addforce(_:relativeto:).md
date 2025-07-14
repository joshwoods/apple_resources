

- RealityKit
- HasPhysicsBody
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

## Discussion

The physics simulator applies the added force until the end of the frame interval. To continue exerting the force after that time, add the force again with another call to the method. Handle the SceneEvents.Update event to receive an indication of when the frame interval ends. For an app that renders at 60 frames per second (fps), this event occurs about once per 16 milliseconds.

## See Also

### Adding and clearing forces

func addForce(SIMD3&lt;Float>, at: SIMD3&lt;Float>, relativeTo: Entity?)

Applies a force to the physics body at the specified position.

func addTorque(SIMD3&lt;Float>, relativeTo: Entity?)

Applies a torque to the physics body at its center of mass.

func clearForcesAndTorques()

Clears all forces previously added to the physics body.

