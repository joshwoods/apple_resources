

- Spatial
-  SphericalCoordinates3D 

Structure

# SphericalCoordinates3D

A structure that defines spherical coordinates in radial, inclination, azimuthal order.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct SphericalCoordinates3D
```

## Topics

### Creating a spherical coordinates structure

init()

Creates a spherical coordinates structure.

init(Vector3D)

Creates a spherical coordinates structure from the Cartesian coordinates represented by the specified simd vector.

init(Point3D)

Creates a spherical coordinates structure from the Cartesian coordinates represented by the specified Spatial point.

init(simd_double3)

Creates a new spherical coordinates structure from the specified Cartesian coordinates represented by a simd vector.

init(radius: Double, inclination: Angle2D, azimuth: Angle2D)

Creates a new spherical coordinates structure with the specified radius, inclination, and azimuth.

init(vector: simd_double3)

Creates a new spherical coordinates structure from the specified Cartesian coordinates represented by a simd vector.

init(x: Double, y: Double, z: Double)

Creates a new spherical coordinates structure from the specified Cartesian coordinates.

### Inspecting a spherical coordinates structure’s properties

var azimuth: Angle2D

The azimuthal angle, in radians.

var inclination: Angle2D

The inclination angle, in radians.

var radius: Double

The distance to the origin.

var vector: simd_double3

A simd three-element vector that contains the radius, inclination, and azimuth values.

var customMirror: Mirror

The custom mirror for this instance.

### Default Implementations

CustomReflectable Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable
- CustomReflectable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### 3D primitives

struct Point3D

A point in a 3D coordinate system.

struct Size3D

A size that describes width, height, and depth in a 3D coordinate system.

struct Rect3D

A rectangle in a 3D coordinate system.

struct Rotation3D

A rotation in three dimensions.

struct RotationAxis3D

A 3D rotation axis.

struct Pose3D

A structure that contains a 3D position and a 3D rotation.

struct ScaledPose3D

A structure that contains a position, rotation, and scale.

struct Ray3D

A ray in a 3D coordinate system.

