

- RealityKit
- PhysicsBodyComponent
-  init(shapes:density:material:mode:) 

Initializer

# init(shapes:density:material:mode:)

Creates a physics body component deriving mass properties from shape and density.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
init(
    shapes: [ShapeResource],
    density: Float,
    material: PhysicsMaterialResource? = nil,
    mode: PhysicsBodyMode = .dynamic
)
```

## Parameters 

`shapes`  

The shape for which to estimate the mass, rotational inertia, and center of mass.

`density`  

The density of the object in kilograms per cubic meter.

`material`  

The material properties, like friction.

`mode`  

The simulation mode that indicates how a body responds to forces.

## Mentioned in 

Designing scene hierarchies for efficient physics simulation

## See Also

### Creating a physics body component

init()

Creates a physics body component with default settings.

init(massProperties: PhysicsMassProperties, material: PhysicsMaterialResource?, mode: PhysicsBodyMode)

Creates a physics body component with the given mass properties, material, and mode.

init(shapes: [ShapeResource], mass: Float, material: PhysicsMaterialResource?, mode: PhysicsBodyMode)

Creates a physics body component deriving mass properties from shape and mass.

