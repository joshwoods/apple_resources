

- Spatial
- SphericalCoordinates3D
-  vector 

Instance Property

# vector

A simd three-element vector that contains the radius, inclination, and azimuth values.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
var vector: simd_double3 { get set }
```

## See Also

### Inspecting a spherical coordinates structure’s properties

var azimuth: Angle2D

The azimuthal angle, in radians.

var inclination: Angle2D

The inclination angle, in radians.

var radius: Double

The distance to the origin.

var customMirror: Mirror

The custom mirror for this instance.

