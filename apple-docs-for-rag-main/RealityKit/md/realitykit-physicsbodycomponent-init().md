

- RealityKit
- PhysicsBodyComponent
-  init() 

Initializer

# init()

Creates a physics body component with default settings.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
init()
```

## Discussion

For the default settings used in a new physics body component, see the discussions of the component’s individual properties.

## See Also

### Creating a physics body component

init(massProperties: PhysicsMassProperties, material: PhysicsMaterialResource?, mode: PhysicsBodyMode)

Creates a physics body component with the given mass properties, material, and mode.

init(shapes: [ShapeResource], density: Float, material: PhysicsMaterialResource?, mode: PhysicsBodyMode)

Creates a physics body component deriving mass properties from shape and density.

init(shapes: [ShapeResource], mass: Float, material: PhysicsMaterialResource?, mode: PhysicsBodyMode)

Creates a physics body component deriving mass properties from shape and mass.

