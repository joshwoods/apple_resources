

- Spatial
-  Ray3D 

Structure

# Ray3D

A ray in a 3D coordinate system.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Ray3D
```

## Topics

### Creating a 3D ray structure

init()

Creates a ray structure.

init(origin: Point3D, direction: Vector3D)

Creates a ray with the specified origin and the specified direction from Spatial primitives.

init(origin: simd_float3, direction: simd_float3)

Creates a ray with the specified origin and the specified direction from single-precision vectors.

init(origin: simd_double3, direction: simd_double3)

Creates a ray with the specified origin and the specified direction from double-precision vectors.

### Inspecting a 3D ray’s properties

var origin: Point3D

The origin of the ray.

var direction: Vector3D

The direction of the ray.

### Transforming a 3D ray structure

func apply(Pose3D)

Applies the specified pose to the ray.

func applying(AffineTransform3D) -> Ray3D

Returns a ray that results from applying the specified affine transform.

func applying(ProjectiveTransform3D) -> Ray3D

Returns a ray that results from applying the specified projective transform.

func applying(Pose3D) -> Ray3D

Returns a ray that results from applying the specified pose.

func unapplying(AffineTransform3D) -> Ray3D

Returns a ray that results from unapplying the specified affine transform.

func unapplying(ProjectiveTransform3D) -> Ray3D

Returns a ray that results from unapplying the specified projective transform.

func unapplying(Pose3D) -> Ray3D

Unapplies the specified pose to the ray.

func rotated(by: Rotation3D) -> Ray3D

Returns a ray that results from applying the specified rotation.

func rotated(by: simd_quatd) -> Ray3D

Returns a ray that results from rotating with the specified quaternion.

func rotated(by: simd_quatd, around: Point3D) -> Ray3D

Returns a ray that’s rotated by the specified quaternion around a specified pivot.

func rotated(by: Rotation3D, around: Point3D) -> Ray3D

Returns a ray that’s rotated by the specified rotation around a specified pivot.

func applying(ScaledPose3D) -> Ray3D

Returns a ray that’s transformed by the specified scaled pose.

func unapplying(ScaledPose3D) -> Ray3D

Returns a ray that’s transformed by the inverse of the specified scaled pose.

### Checking characteristics

var isFinite: Bool

A Boolean value that indicates whether all of the values of the ray are finite.

var isNaN: Bool

A Boolean value that indicates whether the ray contains any NaN values.

var isZero: Bool

A Boolean value that indicates whether all of the values of the ray are zero.

func intersects(Rect3D) -> Bool

Returns a Boolean value that indicates whether a ray intersects a rectangle.

func intersects(sphereOrigin: Point3D, sphereRadius: Double) -> Bool

Returns a Boolean value that indicates whether the ray intersects a specified sphere.

### Comparing values

static func == (Ray3D, Ray3D) -> Bool

Returns a Boolean value that indicates whether two values are equal.

### Applying arithmetic operations

static func * (Pose3D, Ray3D) -> Ray3D

Returns the ray that results from applying the pose to the ray.

### Initializers

init(origin: Point3D, direction: Vector3D)

Creates a ray from Spatial primitives that describe the origin and direction.

### Default Implementations

CustomReflectable Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

Primitive3D Implementations

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
- Primitive3D
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

struct ScaledPose3D

A structure that contains a position, rotation, and scale.

struct SphericalCoordinates3D

A structure that defines spherical coordinates in radial, inclination, azimuthal order.

