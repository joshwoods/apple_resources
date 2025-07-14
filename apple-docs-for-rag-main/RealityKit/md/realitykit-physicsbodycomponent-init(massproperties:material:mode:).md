

- RealityKit
- PhysicsBodyComponent
-  init(massProperties:material:mode:) 

Initializer

# init(massProperties:material:mode:)

Creates a physics body component with the given mass properties, material, and mode.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
init(
    massProperties: PhysicsMassProperties = .default,
    material: PhysicsMaterialResource? = nil,
    mode: PhysicsBodyMode = .dynamic
)
```

## Parameters 

`massProperties`  

The mass properties, like inertia.

`material`  

The material properties, like friction.

`mode`  

The simulation mode that indicates how a body responds to forces.

## See Also

### Creating a physics body component

init()

Creates a physics body component with default settings.

init(shapes: [ShapeResource], density: Float, material: PhysicsMaterialResource?, mode: PhysicsBodyMode)

Creates a physics body component deriving mass properties from shape and density.

init(shapes: [ShapeResource], mass: Float, material: PhysicsMaterialResource?, mode: PhysicsBodyMode)

Creates a physics body component deriving mass properties from shape and mass.

