

- Spatial
-  RotationAxis3D 

Structure

# RotationAxis3D

A 3D rotation axis.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct RotationAxis3D
```

## Topics

### Creating a 3D rotation axis structure

init()

Creates a rotation axis.

init(simd_float3)

Creates a rotation axis from the specified single-precision vector.

init(simd_double3)

Creates a rotation axis from the specified double-precision vector.

init(vector: simd_double3)

Creates a rotation axis from a three-element double-precision vector.

init(Vector3D)

Creates a rotation axis from a Spatial vector.

init(x: Double, y: Double, z: Double)

Creates a rotation axis from the specified double-precision values.

init&lt;T>(x: T, y: T, z: T)

Creates a rotation axis from the specified floating-point values.

### Checking characteristics

var x: Double

The x-coordinate value.

var y: Double

The y-coordinate value.

var z: Double

The z-coordinate value.

var vector: simd_double3

A simd three-element vector that contains the x-, y-, and z-coordinate values.

var isZero: Bool

A Boolean value that indicates whether the rotation axis is zero.

### Constants

static let x: RotationAxis3D

The x-axis, expressed in unit coordinates.

static let y: RotationAxis3D

The y-axis, expressed in unit coordinates.

static let z: RotationAxis3D

The z-axis, expressed in unit coordinates.

static let xy: RotationAxis3D

The xy-axis, expressed in unit coordinates.

static let yz: RotationAxis3D

The yz-axis, expressed in unit coordinates.

static let xz: RotationAxis3D

The xz-axis, expressed in unit coordinates.

static let xyz: RotationAxis3D

The xyz-axis, expressed in unit coordinates.

static let zero: RotationAxis3D

The rotation axis with the zero value.

### Deprecated symbols

var simd: simd_double3

A simd three-element vector that contains the x-, y-, and z-coordinate values.

Deprecated

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

struct Pose3D

A structure that contains a 3D position and a 3D rotation.

struct ScaledPose3D

A structure that contains a position, rotation, and scale.

struct SphericalCoordinates3D

A structure that defines spherical coordinates in radial, inclination, azimuthal order.

struct Ray3D

A ray in a 3D coordinate system.

