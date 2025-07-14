

- Spatial
- SphericalCoordinates3D
-  init(radius:inclination:azimuth:) 

Initializer

# init(radius:inclination:azimuth:)

Creates a new spherical coordinates structure with the specified radius, inclination, and azimuth.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    radius: Double,
    inclination: Angle2D,
    azimuth: Angle2D
)
```

## See Also

### Creating a spherical coordinates structure

init()

Creates a spherical coordinates structure.

init(Vector3D)

Creates a spherical coordinates structure from the Cartesian coordinates represented by the specified simd vector.

init(Point3D)

Creates a spherical coordinates structure from the Cartesian coordinates represented by the specified Spatial point.

init(simd_double3)

Creates a new spherical coordinates structure from the specified Cartesian coordinates represented by a simd vector.

init(vector: simd_double3)

Creates a new spherical coordinates structure from the specified Cartesian coordinates represented by a simd vector.

init(x: Double, y: Double, z: Double)

Creates a new spherical coordinates structure from the specified Cartesian coordinates.

