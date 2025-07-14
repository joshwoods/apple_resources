

- Spatial
-  Size3D 

Structure

# Size3D

A size that describes width, height, and depth in a 3D coordinate system.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Size3D
```

## Topics

### Creating a 3D size structure

init()

Creates a size structure.

init(width: Double, height: Double, depth: Double)

Creates a size structure from the specified double-precision values.

init&lt;T>(width: T, height: T, depth: T)

Creates a size structure from the specified floating-point values.

init(simd_float3)

Creates a size structure from the specified single-precision vector.

init(simd_double3)

Creates a size structure from the specified double-precision vector.

init(vector: simd_double3)

Creates a size structure from the specified double-precision vector.

init(Point3D)

Creates a size structure from the specified Spatial point.

init(Vector3D)

Creates a size structure from the specified Spatial vector.

### Inspecting a 3D size’s properties

var width: Double

The width value.

var height: Double

The height value.

var depth: Double

The depth value.

var size: Size3D

The size value.

var vector: simd_double3

### Transforming a 3D size structure

func applying(Pose3D) -> Size3D

Returns a size that results from applying the specified pose.

func applying(ScaledPose3D) -> Size3D

Returns a size that’s transformed by the specified scaled pose.

func applying(Pose3D) -> Size3D

Returns a size that results from applying the specified pose.

func unapplying(AffineTransform3D) -> Size3D

Returns a size that results from unapplying the specified affine transform.

func unapplying(ProjectiveTransform3D) -> Size3D

Returns a size that results from unapplying the specified projective transform.

func unapplying(Pose3D) -> Size3D

Returns a size that results from unapplying the specified pose.

func sheared(AxisWithFactors) -> Size3D

Returns a size that results from shearing over an axis by shear factors for the other two axes.

func applying(ScaledPose3D) -> Size3D

Returns a size that’s transformed by the specified scaled pose.

func unapplying(ScaledPose3D) -> Size3D

Returns a size that’s transformed by the inverse of the specified scaled pose.

### Checking characteristics

func contains(anyOf: [Point3D]) -> Bool

Returns a Boolean value that indicates whether the size contains the specified point.

### Creating derived 3D sizes

func intersection(Size3D) -> Size3D?

Returns the intersection of two sizes.

### Comparing values

static func == (Size3D, Size3D) -> Bool

Returns a Boolean value that indicates whether two values are equal.

### 3D size constants

static let one: Size3D

The size structure with width, height, and depth values of one.

### Applying arithmetic operations

static func * (Size3D, Double) -> Size3D

Returns a size that’s the product of a size and a scalar value.

static func * (Double, Size3D) -> Size3D

Returns a size that’s the product of a scalar value and a size.

static func * (AffineTransform3D, Size3D) -> Size3D

Returns the size that results from applying the affine transform to the size.

static func * (ProjectiveTransform3D, Size3D) -> Size3D

Returns the size that results from applying the projective transform to the size.

static func * (Pose3D, Size3D) -> Size3D

Returns a new size after applying the pose to the size.

static func + (Size3D, Size3D) -> Size3D

Returns a size that’s the element-wise sum of two sizes.

static func - (Size3D) -> Size3D

Returns a size that’s the element-wise negation of the size.

static func - (Size3D, Size3D) -> Size3D

Returns a size that’s the element-wise difference of two points.

static func *= (inout Size3D, Double)

Multiplies a size and a double-precision value, and stores the result in the left-hand-side variable.

static func += (inout Size3D, Size3D)

Adds two size structures and stores the result in the left-hand-side variable.

static func += (inout Size3D, Vector3D)

Adds a size and a vector, and stores the result in the left-hand-side variable.

static func -= (inout Size3D, Size3D)

Subtracts a size from a size and stores the difference in the left-hand-side variable.

static func -= (inout Size3D, Vector3D)

Subtracts a size from a vector and stores the difference in the left-hand-side variable.

static func / (Size3D, Double) -> Size3D

Returns a size with each element divided by a scalar value.

static func /= (inout Size3D, Double)

Divides a size by a scalar vaue and stores the result in the left-hand-side variable.

### Deprecated symbols

var simd: simd_double3Deprecated

func containsAny(of: [Point3D]) -> Bool

Returns a Boolean value that indicates whether the size contains the specified point.

Deprecated

### Default Implementations

AdditiveArithmetic Implementations

CustomReflectable Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

Primitive3D Implementations

Scalable3D Implementations

Shearable3D Implementations

Volumetric Implementations

## Relationships

### Conforms To

- AdditiveArithmetic
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
- Scalable3D
- Sendable
- Shearable3D
- VectorArithmetic
- Volumetric

## See Also

### 3D primitives

struct Point3D

A point in a 3D coordinate system.

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

