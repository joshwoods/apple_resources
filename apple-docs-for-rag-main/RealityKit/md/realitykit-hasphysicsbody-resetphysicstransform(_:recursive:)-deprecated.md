

- RealityKit
- HasPhysicsBody
-  resetPhysicsTransform(\_:recursive:) Deprecated

Instance Method

# resetPhysicsTransform(\_:recursive:)

Resets the position and velocities of the simulated physics body.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func resetPhysicsTransform(
    _ transform: Transform,
    recursive: Bool = true
)
```

Deprecated

Will be hidden in RealityKit 2019.

## Parameters 

`transform`  

The new transform to inject into the dynamic physics simulation of the entity.

`recursive`  

Apply the reset to child entities.

## Discussion

Call this method to change the transform applied to a body by physics simulation. This only matters for dynamic rigid bodies, with a mode of PhysicsBodyMode.dynamic. This is the only kind of body that’s affected by physics simulations. For all others, modify the entity’s transform property directly.

Conversely, directly modifying the transform of a dynamic body has no effect because the physics simulation overwrites it on every frame.

## See Also

### Resetting physics simulations

func resetPhysicsTransform(recursive: Bool)

Resets the position, orientation, and velocities of the simulated physics body.

