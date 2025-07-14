

- RealityKit
- HasPhysicsBody
-  applyImpulse(\_:at:relativeTo:) 

Instance Method

# applyImpulse(\_:at:relativeTo:)

Applies an impulse to the physics body at the specified position.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func applyImpulse(
    _ impulse: SIMD3,
    at position: SIMD3,
    relativeTo referenceEntity: Entity?
)
```

## Parameters 

`impulse`  

An impulse in newton seconds.

`position`  

The position at which to apply the impulse.

`referenceEntity`  

The reference entity that defines the coordinate space in which `position` and `impulse` are defined.

## See Also

### Applying impulses

func applyLinearImpulse(SIMD3&lt;Float>, relativeTo: Entity?)

Applies an impulse to the physics body at its center of mass.

func applyAngularImpulse(SIMD3&lt;Float>, relativeTo: Entity?)

Applies an angular (torque) impulse to the physics body at its center of mass.

