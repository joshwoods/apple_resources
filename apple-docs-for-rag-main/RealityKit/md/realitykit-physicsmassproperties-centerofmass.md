

- RealityKit
- PhysicsMassProperties
-  centerOfMass 

Instance Property

# centerOfMass

The position of the center of mass and the orientation of the principal axes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
var centerOfMass: (position: SIMD3, orientation: simd_quatf)
```

## Discussion

The `position` defines the center of mass with a default value of `(0, 0, 0)`, which means that the local origin of the model is the center of mass.

The `orientation` defines the principal axes, such the inertia matrix is a diagonal.

## See Also

### Getting mass properties

var mass: Float

The mass in kilograms.

var inertia: SIMD3&lt;Float>

The inertia in kilograms per square meter.

