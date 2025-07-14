

- RealityKit
- PhysicsMassProperties
-  mass 

Instance Property

# mass

The mass in kilograms.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
var mass: Float
```

## Discussion

For a mass of `0` or infinity, the simulation treats the object as PhysicsBodyMode.kinematic. That is, the object doesn’t respond to forces.

## See Also

### Getting mass properties

var inertia: SIMD3&lt;Float>

The inertia in kilograms per square meter.

var centerOfMass: (position: SIMD3&lt;Float>, orientation: simd_quatf)

The position of the center of mass and the orientation of the principal axes.

