

- Spatial
- SphericalCoordinates3D
-  init(\_:) 

Initializer

# init(\_:)

Creates a new spherical coordinates structure from the specified Cartesian coordinates represented by a simd vector.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
init(_ vector: simd_double3)
```

## See Also

### Creating a spherical coordinates structure

init()

Creates a spherical coordinates structure.

init(Vector3D)

Creates a spherical coordinates structure from the Cartesian coordinates represented by the specified simd vector.

init(Point3D)

Creates a spherical coordinates structure from the Cartesian coordinates represented by the specified Spatial point.

init(radius: Double, inclination: Angle2D, azimuth: Angle2D)

Creates a new spherical coordinates structure with the specified radius, inclination, and azimuth.

init(vector: simd_double3)

Creates a new spherical coordinates structure from the specified Cartesian coordinates represented by a simd vector.

init(x: Double, y: Double, z: Double)

Creates a new spherical coordinates structure from the specified Cartesian coordinates.

