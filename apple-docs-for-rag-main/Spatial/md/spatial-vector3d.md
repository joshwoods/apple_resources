

- Spatial
-  Vector3D 

Structure

# Vector3D

A three-element vector.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Vector3D
```

## Topics

### Creating a vector

init()

Creates a vector.

init(x: Double, y: Double, z: Double)

Creates a vector from the specified double-precision values.

init&lt;T>(x: T, y: T, z: T)

Creates a vector from the specified floating-point values.

init(simd_float3)

Creates a ray from the specified single-precision vector.

init(simd_double3)

Creates a vector from the specified double-precision vector.

init(vector: simd_double3)

Creates a vector from the specified double-precision vector.

init(RotationAxis3D)

Creates a vector from the specified Spatial rotation axis.

init(Point3D)

Creates a vector from the specified Spatial point structure.

init(Size3D)

Creates a vector from the specified Spatial size structure.

init(SphericalCoordinates3D)

Creates a vector from the specified Spatial spherical coordinates structure.

### Inspecting a vector’s properties

var x: Double

The x-element value.

var y: Double

The y-element value.

var z: Double

The z-element value.

var vector: simd_double3

A simd three-element vector that contains the x-, y-, and z-element values.

### Checking characteristics

func rotation(to: Vector3D) -> Rotation3D

Returns the rotation from the normalized first vector to the normalized second vector.

### Geometry functions

func cross(Vector3D) -> Vector3D

Returns the cross product of the vector and the specified vector.

func dot(Vector3D) -> Double

Returns the dot product of the vector and the specified vector.

var length: Double

The length of the vector.

var lengthSquared: Double

The square of the length of the vector.

func normalize()

Normalizes the mutable vector.

var normalized: Vector3D

A new vector that represents the normalized copy of the current vector.

func projected(Vector3D) -> Vector3D

Returns the vector projected onto the specified vector.

func reflected(Vector3D) -> Vector3D

Returns the reflection direction of the incident vector and a specified unit normal vector.

### Transforming a vector

func applying(AffineTransform3D) -> Vector3D

Returns the vector resulting from applying an affine transform to the vector.

func applying(ProjectiveTransform3D) -> Vector3D

Returns the vector resulting from applying a projective transform to the vector.

func applying(Pose3D) -> Vector3D

Returns a vector that results from applying the specified pose.

func unapplying(AffineTransform3D) -> Vector3D

Returns the vector resulting from unapplying an affine transform to the vector.

func unapplying(ProjectiveTransform3D) -> Vector3D

Returns the vector resulting from unapplying a projective transform to the vector.

func unapplying(Pose3D) -> Vector3D

Returns a vector that results from unapplying the specified pose.

func rotated(by: Rotation3D) -> Vector3D

Returns the vector rotated by the specified rotation around the origin.

func rotated(by: simd_quatd) -> Vector3D

Returns the vector rotated by the specified quaternion around the origin.

func scaled(by: Size3D) -> Vector3D

Returns the vector scaled by the specified size.

func scaledBy(x: Double, y: Double, z: Double) -> Vector3D

Returns a vector that results from scaling with the specified double-precision values.

func uniformlyScaled(by: Double) -> Vector3D

Returns the entity uniformly scaled by the specified scalar value.

func sheared(AxisWithFactors) -> Vector3D

Returns a vector that results from shearing over an axis by shear factors for the other two axes.

func applying(ScaledPose3D) -> Vector3D

Returns a vector that’s transformed by the specified scaled pose.

func unapplying(ScaledPose3D) -> Vector3D

Returns a vector that’s transformed by the inverse of the specified scaled pose.

### Comparing values

static func == (Vector3D, Vector3D) -> Bool

Returns a Boolean value that indicates whether two values are equal.

### Encoding and decoding a vector

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

### Type properties

static let forward: Vector3D

A vector that contains the values 0, 0, 1.

static let right: Vector3D

A vector that contains the values 1, 0, 0.

static let up: Vector3D

A vector that contains the values 0, 1, 0.

### Applying arithmetic operations

static func * (Vector3D, Double) -> Vector3D

Returns a vector that’s the product of a vector and a scalar value.

static func * (Double, Vector3D) -> Vector3D

Returns a vector that’s the product of a scalar value and a vector.

static func * (AffineTransform3D, Vector3D) -> Vector3D

Returns the vector that results from applying the affine transform to the vector.

static func * (ProjectiveTransform3D, Vector3D) -> Vector3D

Returns the vector that results from applying the projective transform to the vector.

static func * (Pose3D, Vector3D) -> Vector3D

Returns a new vector after applying the pose to the vector.

static func + (Vector3D, Vector3D) -> Vector3D

Returns a vector that’s the element-wise sum of two sizes.

static func + (Vector3D, Size3D) -> Size3D

Returns a vector that’s the element-wise sum of a vector and a size.

static func + (Size3D, Vector3D) -> Size3D

Returns a vector that’s the element-wise sum of a size and a vector.

static func + (Vector3D, Point3D) -> Point3D

Returns a vector that’s the element-wise sum of a vector and a point.

static func + (Point3D, Vector3D) -> Point3D

Returns a vector that’s the element-wise sum of a point and a vector.

static func - (Vector3D) -> Vector3D

Returns a vector that’s the element-wise negation of the vector.

static func - (Vector3D, Vector3D) -> Vector3D

Returns a size that’s the element-wise difference of two vectors.

static func - (Vector3D, Size3D) -> Size3D

Returns a size that’s the element-wise difference of a vector and a size.

static func - (Size3D, Vector3D) -> Size3D

Returns a size that’s the element-wise difference of a size and a vector.

static func - (Vector3D, Point3D) -> Point3D

Returns a size that’s the element-wise difference of a vector and a point.

static func - (Point3D, Vector3D) -> Point3D

Returns a size that’s the element-wise difference of a point and a vector.

static func *= (inout Vector3D, Double)

Multiplies a vector and a double-precision value, and stores the result in the left-hand-side variable.

static func += (inout Vector3D, Vector3D)

Adds two vectors and stores the result in the left-hand-side variable.

static func -= (inout Vector3D, Vector3D)

Subtracts a vector from a vector and stores the difference in the left-hand-side variable.

static func / (Vector3D, Double) -> Vector3D

Returns a vector with each element divided by a scalar value.

static func /= (inout Vector3D, Double)

Divides a vector by a scalar value and stores the result in the left-hand-side variable.

### Default Implementations

AdditiveArithmetic Implementations

CustomReflectable Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

Primitive3D Implementations

Rotatable3D Implementations

Scalable3D Implementations

Shearable3D Implementations

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

## See Also

### Data structures

struct Axis3D

Constants that describe an axis.

