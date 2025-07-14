

- RealityKit
- PhysicsMaterialResource
-  generate(friction:restitution:) 

Type Method

# generate(friction:restitution:)

Generates a new material with the given characteristics.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
static func generate(
    friction: Float = 0.8,
    restitution: Float = 0.8
) -> PhysicsMaterialResource
```

## Parameters 

`friction`  

The coefficient of friction, in the range `[0, infinity)`.

`restitution`  

The coefficient of restitution, in the range `[0, 1]`. Use values at the high end of the range to indicate materials that experience elastic collisions, meaning that objects bounce off each other and kinetic energy is conserved after a collision. Use low values to indicate materials that lose kinetic energy when they collide.

## Return Value

A physics material resource.

## See Also

### Creating a custom material resource

static func generate(staticFriction: Float, dynamicFriction: Float, restitution: Float) -> PhysicsMaterialResource

Creates a new material with the specified static friction, dynamic friction, and restitution.

