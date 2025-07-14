

- Spatial
-  Pose3D 

Structure

# Pose3D

A structure that contains a 3D position and a 3D rotation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Pose3D
```

## Topics

### Creating a 3D pose structure

init()

Creates a pose structure.

init?(simd_float4x4)

Creates a pose from the specified 4 x 4 single-precision matrix.

init?(simd_double4x4)

Creates a pose from the specified 4 x 4 double-precision matrix.

init(forward: Vector3D, up: Vector3D)

Creates a pose with the specified forward and up vectors.

init(position: simd_float3, rotation: simd_quatf)

Creates a pose with the specified single-precision position vector and quaternion.

init(position: Point3D, rotation: Rotation3D)

Creates a pose with the specified Spatial position and rotation structures.

init(position: Point3D, rotation: Rotation3D)

Creates a pose with the specified single-precision position vector and quaternion.

init(position: simd_double3, rotation: simd_quatd)

Creates a pose with the specified double-precision position vector and quaternion.

init(position: Point3D, target: Point3D, up: Vector3D)

Returns a pose at the specified position with the rotation towards the target.

init?(transform: AffineTransform3D)

Returns a pose with a position and rotation defined by an affine transform.

init?(transform: ProjectiveTransform3D)

Returns a pose with a position and rotation defined by a projective transform.

### Constants

static var identity: Pose3D

The identity pose.

### Inspecting a 3D pose’s properties

var matrix: simd_double4x4

The pose’s underlying matrix.

var position: Point3D

The pose’s position.

var rotation: Rotation3D

The pose’s rotation.

var inverse: Pose3D

The pose’s inverse.

### Transforming a 3D pose structure

func concatenating(ScaledPose3D) -> ScaledPose3D

Returns a pose that represents the concatenation of a scaled pose and a pose.

func concatenating(Pose3D) -> Pose3D

Returns a pose that represents the concatenation of two poses.

func flip(along: Axis3D)

Flips a pose along the specified axis.

func flipped(along: Axis3D) -> Pose3D

Returns a pose that results from flipping it along the specified axis.

func rotated(by: simd_quatd) -> Pose3D

Returns a pose that results from rotating with the specified quaternion.

func rotated(by: Rotation3D) -> Pose3D

Returns a pose that results from applying the specified rotation.

### Checking characteristics

var isIdentity: Bool

A Boolean value that indicates whether the pose is the identity pose.

### Comparing values

func isApproximatelyEqual(to: Pose3D, tolerance: Double) -> Bool

Returns a Boolean value that indicates whether two poses are equal within a specified tolerance.

static func == (Pose3D, Pose3D) -> Bool

Returns a Boolean value that indicates whether two values are equal.

### Applying arithmetic operations

static func * (Pose3D, Pose3D) -> Pose3D

Returns the concatenation of two poses.

static func *= (inout Pose3D, Pose3D)

Concatenates two poses and stores the result in the left-hand-side variable.

### Deprecated symbols

init?(matrix: simd_float4x4)Deprecated

init?(matrix: simd_double4x4)Deprecated

### Default Implementations

CustomReflectable Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

Rotatable3D Implementations

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
- Translatable3D

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

struct ScaledPose3D

A structure that contains a position, rotation, and scale.

struct SphericalCoordinates3D

A structure that defines spherical coordinates in radial, inclination, azimuthal order.

struct Ray3D

A ray in a 3D coordinate system.

