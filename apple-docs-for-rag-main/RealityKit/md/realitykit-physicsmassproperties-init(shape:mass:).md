

- RealityKit
- PhysicsMassProperties
-  init(shape:mass:) 

Initializer

# init(shape:mass:)

Creates the mass properties for a solid shape with the specified mass.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
init(
    shape: ShapeResource,
    mass: Float
)
```

## Parameters 

`shape`  

The shape for which to calculate the mass frame.

`mass`  

The mass of the object in kilograms.

## See Also

### Creating custom mass properties

init()

Creates a mass properties instance with default settings.

init(mass: Float, inertia: SIMD3&lt;Float>, centerOfMass: (position: SIMD3&lt;Float>, orientation: simd_quatf))

Creates a mass properties instance with the given settings.

init(shape: ShapeResource, density: Float)

Creates the mass properties for a solid shape with the specified density.

