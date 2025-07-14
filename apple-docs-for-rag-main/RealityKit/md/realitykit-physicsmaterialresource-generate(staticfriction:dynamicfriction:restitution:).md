

- RealityKit
- PhysicsMaterialResource
-  generate(staticFriction:dynamicFriction:restitution:) 

Type Method

# generate(staticFriction:dynamicFriction:restitution:)

Creates a new material with the specified static friction, dynamic friction, and restitution.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15.4+visionOS

``` source
@MainActor @preconcurrency
static func generate(
    staticFriction: Float,
    dynamicFriction: Float,
    restitution: Float
) -> PhysicsMaterialResource
```

## Parameters 

`staticFriction`  

The static (stationary) friction coefficient in the range \[0, ∞).

`dynamicFriction`  

The dynamic (moving) friction coefficient in the range \[0, ∞).

`restitution`  

The coefficient of restitution (bounciness) in the range \[0, 1\].

## See Also

### Creating a custom material resource

static func generate(friction: Float, restitution: Float) -> PhysicsMaterialResource

Generates a new material with the given characteristics.

