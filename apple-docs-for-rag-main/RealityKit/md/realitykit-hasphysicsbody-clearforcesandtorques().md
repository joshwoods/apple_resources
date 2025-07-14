

- RealityKit
- HasPhysicsBody
-  clearForcesAndTorques() 

Instance Method

# clearForcesAndTorques()

Clears all forces previously added to the physics body.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func clearForcesAndTorques()
```

## See Also

### Adding and clearing forces

func addForce(SIMD3&lt;Float>, relativeTo: Entity?)

Applies a force to the physics body at its center of mass.

func addForce(SIMD3&lt;Float>, at: SIMD3&lt;Float>, relativeTo: Entity?)

Applies a force to the physics body at the specified position.

func addTorque(SIMD3&lt;Float>, relativeTo: Entity?)

Applies a torque to the physics body at its center of mass.

