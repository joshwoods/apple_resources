

- RealityKit
- HasPhysicsBody
-  applyAngularImpulse(\_:relativeTo:) 

Instance Method

# applyAngularImpulse(\_:relativeTo:)

Applies an angular (torque) impulse to the physics body at its center of mass.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func applyAngularImpulse(
    _ impulse: SIMD3,
    relativeTo referenceEntity: Entity?
)
```

## Parameters 

`impulse`  

An angular impulse in kilogram square meters per second.

`referenceEntity`  

The reference entity that defines the coordinate space in which `impulse` is defined.

## See Also

### Applying impulses

func applyLinearImpulse(SIMD3&lt;Float>, relativeTo: Entity?)

Applies an impulse to the physics body at its center of mass.

func applyImpulse(SIMD3&lt;Float>, at: SIMD3&lt;Float>, relativeTo: Entity?)

Applies an impulse to the physics body at the specified position.

