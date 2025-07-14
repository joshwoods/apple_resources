

- RealityKit
- PhysicsMassProperties
-  init() 

Initializer

# init()

Creates a mass properties instance with default settings.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
init()
```

## See Also

### Creating custom mass properties

init(mass: Float, inertia: SIMD3&lt;Float>, centerOfMass: (position: SIMD3&lt;Float>, orientation: simd_quatf))

Creates a mass properties instance with the given settings.

init(shape: ShapeResource, density: Float)

Creates the mass properties for a solid shape with the specified density.

init(shape: ShapeResource, mass: Float)

Creates the mass properties for a solid shape with the specified mass.

