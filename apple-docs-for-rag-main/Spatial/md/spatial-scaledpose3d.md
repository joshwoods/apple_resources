

- Spatial
-  ScaledPose3D 

Structure

# ScaledPose3D

A structure that contains a position, rotation, and scale.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct ScaledPose3D
```

## Topics

### Creating a 3D scaled-pose structure

init()

Creates a scaled pose structure.

init?(simd_float4x4)

Creates a scaled pose from the specified 4 x 4 single-precision matrix.

init?(simd_double4x4)

Creates a scaled pose from the specified 4 x 4 double-precision matrix.

init(forward: Vector3D, scale: Double, up: Vector3D)

Creates a scaled pose with the specified forward and up vectors.

init(position: simd_float3, rotation: simd_quatf, scale: Float)

Creates a scaled pose with the specified single-precision position vector and quaternion.

init(position: simd_double3, rotation: simd_quatd, scale: Double)

Creates a scaled pose with the specified double-precision position vector and quaternion.

init(position: Point3D, target: Point3D, scale: Double, up: Vector3D)

Returns a scaled pose at the specified position with the rotation toward the target.

init(position: Point3D, rotation: Rotation3D, scale: Double)

Creates a pose with the specified Spatial position, rotation, and scale structures.

init(position: Point3D, rotation: Rotation3D, scale: Double)

Creates a scaled pose with the specified double-precision position vector and quaternion.

init?(transform: AffineTransform3D)

Returns a scaled pose with a position, rotation, and scale defined by an affine transform.

init?(transform: ProjectiveTransform3D)

Returns a scaled pose with a position, rotation, and scale defined by a projective transform.

### Inspecting a 3D scaled pose’s properties

var matrix: simd_double4x4

The scaled pose’s underlying matrix.

var position: Point3D

The scaled pose’s position.

var rotation: Rotation3D

The scaled pose’s rotation.

var scale: Double

The scaled pose’s scale.

var inverse: ScaledPose3D

The scaled pose’s inverse.

var customMirror: Mirror

A mirror that reflects the notification.

static var identity: ScaledPose3D

The identity scaled pose.

### Transforming a 3D scaled-pose structure

func flip(along: Axis3D)

Flips a scaled pose along the specified axis.

func flipped(along: Axis3D) -> ScaledPose3D

Returns a scaled pose that results from flipping it along the specified axis.

func rotated(by: simd_quatd) -> ScaledPose3D

Returns a scaled pose that results from rotating with the specified quaternion.

func rotated(by: Rotation3D) -> ScaledPose3D

Returns a scaled pose that results from applying the specified rotation.

func concatenating(ScaledPose3D) -> ScaledPose3D

Returns a scaled pose that represents the concatenation of two scaled poses.

func concatenating(Pose3D) -> ScaledPose3D

Returns a scaled pose that represents the concatenation of two poses.

### Checking characteristics

var isIdentity: Bool

Returns a Boolean value that indicates whether the scaled pose is the identity transform.

### Comparing values

func isApproximatelyEqual(to: ScaledPose3D, tolerance: Double) -> Bool

Returns a Boolean value that indicates whether two scaled poses are equal within a specified tolerance.

static func == (ScaledPose3D, ScaledPose3D) -> Bool

Returns a Boolean value that indicates whether two values are equal.

### Applying arithmetic operations

static func * (ScaledPose3D, ScaledPose3D) -> ScaledPose3D

Returns the concatenation of two scaled poses.

static func * (ScaledPose3D, Pose3D) -> ScaledPose3D

Returns the concatenation of a scaled pose and a pose.

static func * (Pose3D, ScaledPose3D) -> ScaledPose3D

Returns the concatenation of a pose and a scaled pose.

static func *= (inout ScaledPose3D, ScaledPose3D)

Concatenates two scaled poses and stores the result in the left-hand-side variable.

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

struct Pose3D

A structure that contains a 3D position and a 3D rotation.

struct SphericalCoordinates3D

A structure that defines spherical coordinates in radial, inclination, azimuthal order.

struct Ray3D

A ray in a 3D coordinate system.

