

- Spatial
-  Point3D 

Structure

# Point3D

A point in a 3D coordinate system.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Point3D
```

## Topics

### Creating a 3D point structure

init()

Creates a point.

init(x: Double, y: Double, z: Double)

Creates a point from the specified double-precision values.

init&lt;T>(x: T, y: T, z: T)

Creates a point from the specified floating-point values.

init(vector: simd_double3)

Creates a point from the specified double-precision vector.

init(Size3D)

Creates a point from the specified Spatial size structure.

init(simd_float3)

Creates a point from the specified single-precision vector.

init(Vector3D)

Creates a point from the specified Spatial vector.

init(simd_double3)

Creates a point from the specified double-precision vector.

init(SphericalCoordinates3D)

Returns a Spatial point that represents the Cartesian coordinates of the specified spherical coordinates structure.

### Inspecting a 3D point’s properties

var x: Double

The x-coordinate value.

var y: Double

The y-coordinate value.

var z: Double

The z-coordinate value.

var vector: simd_double3

var magnitudeSquared: Double

### Checking characteristics

func distance(to: Point3D) -> Double

Returns the distance between two points.

### Transforming a 3D point structure

func applying(ScaledPose3D) -> Point3D

Returns a point that’s transformed by the specified scaled pose.

func applying(ScaledPose3D) -> Point3D

Returns a point that’s transformed by the specified scaled pose.

func applying(Pose3D) -> Point3D

Returns a point that results from applying the specified pose.

func clamp(to: Rect3D)

Clamps the mutable point to the specified rectangle.

func clamped(to: Rect3D) -> Point3D

Returns a point with coordinates that clamp to the specified rectangle.

func scale(by: Double)

func rotated(by: Rotation3D, around: Point3D) -> Point3D

Returns a point that results from applying a rotation around the specified point.

func rotated(by: simd_quatd, around: Point3D) -> Point3D

Returns a point that results from rotating with a quaternion around the specified point.

func unapplying(Pose3D) -> Point3D

Returns a point that results from unapplying the specified pose.

func unapplying(ScaledPose3D) -> Point3D

Returns a point that’s transformed by the inverse of the specified scaled pose.

func unapplying(ScaledPose3D) -> Point3D

Returns a point that’s transformed by the inverse of the specified scaled pose.

### Comparing values

static func == (Point3D, Point3D) -> Bool

Returns a Boolean value that indicates whether two values are equal.

func isApproximatelyEqual(to: Point3D, tolerance: Double) -> Bool

### Applying arithmetic operations

static func * (Point3D, Double) -> Point3D

Returns a point that’s the product of a point and a scalar value.

static func * (Double, Point3D) -> Point3D

Returns a point that’s the product of a scalar value and a point.

static func * (AffineTransform3D, Point3D) -> Point3D

Returns the point that results from applying the affine transform to the point.

static func * (ProjectiveTransform3D, Point3D) -> Point3D

Returns the point that results from applying the projective transform to the point.

static func * (Pose3D, Point3D) -> Point3D

Returns a new point after applying the pose to the point.

static func + (Point3D, Size3D) -> Point3D

Returns a point that’s the element-wise sum of a point and a size.

static func + (Size3D, Point3D) -> Point3D

Returns a point that’s the element-wise sum of a size and a point.

static func - (Point3D) -> Point3D

Returns a point that’s the element-wise negation of the point.

static func - (Point3D, Size3D) -> Point3D

Returns a point that’s the element-wise difference of a point and a size.

static func - (Point3D, Point3D) -> Vector3D

Returns a point that’s the element-wise difference of two points.

static func - (Size3D, Point3D) -> Point3D

Returns a point that’s the element-wise difference of a size and a point.

static func += (inout Point3D, Vector3D)

Adds a point and a vector, and stores the result in the left-hand-side variable.

static func += (inout Point3D, Size3D)

Adds a point and a size, and stores the result in the left-hand-side variable.

static func -= (inout Point3D, Vector3D)

Subtracts a vector from a point and stores the difference in the left-hand-side variable.

static func -= (inout Point3D, Size3D)

Subtracts a vector from a point and stores the difference in the left-hand-side variable.

static func *= (inout Point3D, Double)

Multiplies a point and a double-precision value, and stores the result in the left-hand-side variable.

static func / (Point3D, Double) -> Point3D

Returns a point with each element divided by a scalar value.

static func /= (inout Point3D, Double)

Divides a point by a scalar value and stores the result in the left-hand-side variable.

### Deprecated symbols

func rotation(to: Point3D) -> Rotation3D

Returns the rotation around the origin from the first point to the second point.

Deprecated

var origin: Point3DDeprecated

var simd: simd_double3

A simd three-element vector that contains the x-, y-, and z-coordinate values.

Deprecated

### Default Implementations

Animatable Implementations

CustomReflectable Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

Primitive3D Implementations

## Relationships

### Conforms To

- Animatable
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

struct Ray3D

A ray in a 3D coordinate system.

