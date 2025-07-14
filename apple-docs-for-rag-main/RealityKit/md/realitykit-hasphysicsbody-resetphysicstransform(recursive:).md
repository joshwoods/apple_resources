

- RealityKit
- HasPhysicsBody
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

### Resetting physics simulations

func resetPhysicsTransform(Transform, recursive: Bool)

Resets the position and velocities of the simulated physics body.

Deprecated

