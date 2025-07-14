

- Spatial
- SphericalCoordinates3D
-  customMirror 

Instance Property

# customMirror

The custom mirror for this instance.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
var customMirror: Mirror { get }
```

## See Also

### Inspecting a spherical coordinates structure’s properties

var azimuth: Angle2D

The azimuthal angle, in radians.

var inclination: Angle2D

The inclination angle, in radians.

var radius: Double

The distance to the origin.

var vector: simd_double3

A simd three-element vector that contains the radius, inclination, and azimuth values.

