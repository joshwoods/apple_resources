

- RealityKit
- PhysicsMassProperties
-  inertia 

Instance Property

# inertia

The inertia in kilograms per square meter.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
var inertia: SIMD3
```

## Discussion

The vector contains the diagonal elements of the diagonalized inertia matrix.

## See Also

### Getting mass properties

var mass: Float

The mass in kilograms.

var centerOfMass: (position: SIMD3&lt;Float>, orientation: simd_quatf)

The position of the center of mass and the orientation of the principal axes.

