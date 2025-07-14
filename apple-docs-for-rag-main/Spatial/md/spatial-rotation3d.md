

- Spatial
-  Rotation3D 

Structure

# Rotation3D

A rotation in three dimensions.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Rotation3D
```

## Topics

### Creating a 3D rotation structure

init()

Creates a rotation.

init()

Creates a rotation structure.

init(eulerAngles: EulerAngles)

Creates a rotation structure with the specified Euler angles.

init(eulerAngles: EulerAngles)

Creates a rotation structure with the specified Euler angles.

struct EulerAngles

A vector that represents three Euler angles and specifies the angle ordering.

init(quaternion: simd_quatd)

Creates a rotation axis from the specified double-precision quaternion.

init(simd_quatd)

Creates a rotation from the specified double-precision quaternion.

init(simd_quatf)

Creates a rotation axis from the specified single-precision quaternion.

init(angle: Angle2D, axis: RotationAxis3D)

Creates a rotation structure with the specified axis and the specified angle from Spatial structures.

init(position: Point3D, target: Point3D, up: Vector3D)

Creates a rotation structure that represents the look-at direction from a position to a target.

init(forward: Vector3D)

Creates a rotation with the specified forward vector.

init(forward: Vector3D, up: Vector3D)

Creates a rotation with the specified forward and up vectors.

init(forward: Vector3D, up: Vector3D)

Creates a rotation with the specified forward and up vectors.

### Inspecting a 3D rotation’s properties

var angle: Angle2D

The angle of the rotation.

var axis: RotationAxis3D

The axis of the rotation.

func eulerAngles(order: __SPEulerAngleOrder) -> EulerAngles

Returns a rotation’s Euler angles.

struct EulerAngles

A vector that represents three Euler angles and specifies the angle ordering.

var quaternion: simd_quatd

A quaternion that represents the rotation.

var vector: simd_double4

The underlying vector of the rotation.

### Transforming a 3D rotation structure

static func slerp(from: Rotation3D, to: Rotation3D, t: Double, along: Rotation3D.SlerpPath) -> Rotation3D

Returns the spherical linear interpolation along either the shortest or the longest arc between two rotations.

enum SlerpPath

Constants that define the arc that a slerp operation takes.

var inverse: Rotation3D

The inverse of the rotation.

static let identity: Rotation3D

The identity rotation.

### Decomposing a 3D rotation structure

func swing(twistAxis: RotationAxis3D) -> Rotation3D

Returns the swing component of the rotation’s swing-twist decomposition for a given twist axis.

func twist(twistAxis: RotationAxis3D) -> Rotation3D

Returns the twist component of the rotation’s swing-twist decomposition for a given twist axis.

func swingTwist(twistAxis: RotationAxis3D) -> (swing: Rotation3D, twist: Rotation3D)

Returns the rotation’s swing-twist decomposition for a given twist axis.

func swing(twistAxis: RotationAxis3D) -> Rotation3D

Returns the swing component of the rotation’s swing-twist decomposition for a given twist axis.

func twist(twistAxis: RotationAxis3D) -> Rotation3D

Returns the twist component of the rotation’s swing-twist decomposition for a given twist axis.

### Checking characteristics

var isIdentity: Bool

A Boolean value that indicates whether the rotation is the identity rotation.

var isIdentity: Bool

A Boolean value that indicates whether the rotation is the identity rotation.

### Comparing values

func isApproximatelyEqual(to: Rotation3D, tolerance: Double) -> Bool

static func == (Rotation3D, Rotation3D) -> Bool

Returns a Boolean value that indicates whether two values are equal.

### Applying arithmetic operations

static func * (Rotation3D, Rotation3D) -> Rotation3D

Returns the product of two rotations.

static func * (Rotation3D, Double) -> Rotation3D

Returns the spherical linear interpolation between the identity rotation and the left-hand-side rotation at the right-hand-side interpolation parameter.

static func * (Double, Rotation3D) -> Rotation3D

Returns the spherical linear interpolation between the identity rotation and the right-hand-side rotation at the left-hand-side interpolation parameter.

func * &lt;T>(Rotation3D, T) -> T

Returns the rotatable entity that results from applying the rotatable entity.

static func *= (inout Rotation3D, Rotation3D)

Computes the product of two rotations and stores the result in the left-hand-side variable.

### Interpolating a 3D rotation structure

static func spline(leftEndpoint: Rotation3D, from: Rotation3D, to: Rotation3D, rightEndpoint: Rotation3D, t: Double) -> Rotation3D

Returns an interpolated value between two rotations along a spherical cubic spline.

### Deprecated symbols

init(Angle2D, Angle2D, Angle2D, order: EulerAngles.Order)

Creates a new Euler angles structure from the specified angle structures and order.

Deprecated

init(eye: Point3D, target: Point3D, up: Vector3D)

Creates a rotation structure that’s the look-at direction from a position to a target.

Deprecated

init(axis: RotationAxis3D, angle: Angle2D)

Creates a rotation structure with the specified axis and the specified angle from Spatial structures.

Deprecated

init(quaternion: simd_quatf)

Creates a rotation axis from the specified single-precision quaternion.

Deprecated

static let zero: Rotation3D

The rotation with the zero value.

Deprecated

var isZero: Bool

A Boolean value that indicates whether the rotation is zero.

Deprecated

### Initializers

init(quaternion: simd_quatd)Deprecated

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
- Rotatable3D
- Sendable

## See Also

### 3D primitives

struct Point3D

A point in a 3D coordinate system.

struct Size3D

A size that describes width, height, and depth in a 3D coordinate system.

struct Rect3D

A rectangle in a 3D coordinate system.

struct RotationAxis3D

A 3D rotation axis.

struct Pose3D

A structure that contains a 3D position and a 3D rotation.

struct ScaledPose3D

A structure that contains a position, rotation, and scale.

struct SphericalCoordinates3D

A structure that defines spherical coordinates in radial, inclination, azimuthal order.

struct Ray3D

A ray in a 3D coordinate system.

