

- Spatial
-  Rect3D 

Structure

# Rect3D

A rectangle in a 3D coordinate system.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Rect3D
```

## Topics

### Creating a 3D rectangle structure

init()

Creates a rectangle structure.

init(BoundingBox)

Creates a rectangle structure from a bounding box.

init(center: Point3D, size: Size3D)

Creates a rectangle with the specified center and the specified size from Spatial structures.

init(center: simd_double3, size: simd_double3)

Creates a rectangle with the specified center and the specified size from double-precision vectors.

init(center: Vector3D, size: Vector3D)

Creates a rectangle with the specified center and the specified size from Spatial vectors.

init(center: simd_float3, size: simd_float3)

Creates a rectangle with the specified center and the specified size from single-precision vectors.

init(origin: simd_double3, size: simd_double3)

Creates a rectangle at the specified origin with the specified size from double-precision vectors.

init(origin: simd_float3, size: simd_float3)

Creates a rectangle at the specified origin with the specified size from single-precision vectors.

init(origin: Vector3D, size: Vector3D)

Creates a rectangle with the specified origin and the specified size from Spatial vectors.

init(origin: Point3D, size: Size3D)

Creates a rectangle at the specified origin and the specified size from Spatial structures.

init(origin: Point3D, size: Size3D)

Creates a rectangle structure.

init(points: [Point3D])

Creates a rectangle that’s the bounding box of the specified points.

### Inspecting a 3D rectangle’s properties

var center: Point3D

The center of the rectangle.

var cornerPoints: [Point3D]

The corner points of the rectangle.

var max: Point3D

A point that represents the corner of the rectangle with the largest x-, y-, and z-coordinates.

var min: Point3D

A point that represents the corner of the rectangle with the smallest x-, y-, and z-coordinates.

var origin: Point3D

The origin of the rectangle.

### Transforming a 3D rectangle structure

func applying(Pose3D) -> Rect3D

Returns a rectangle that results from applying the specified pose.

func applying(ScaledPose3D) -> Rect3D

Returns a rectangle that’s transformed by the specified scaled pose.

func applying(ScaledPose3D) -> Rect3D

Returns a rectangle that’s transformed by the specified scaled pose.

func rotated(by: Rotation3D, around: Point3D) -> Rect3D

Returns a rectangle that results from applying the specified rotation around a pivot point.

func rotated(by: simd_quatd, around: Point3D) -> Rect3D

Returns a rectangle that results from rotating with the specified quaternion around a pivot point.

func scaledBy(x: Double, y: Double, z: Double) -> Rect3D

Returns a rectangle that results from scaling with the specified double-precision values.

func sheared(AxisWithFactors) -> Rect3D

Returns a rectangle that results from shearing over an axis by shear factors for the other two axes.

func unapplying(ProjectiveTransform3D) -> Rect3D

Returns a rectangle that results from unapplying the specified projective transform.

func unapplying(ScaledPose3D) -> Rect3D

Returns a rectangle that’s transformed by the inverse of the specified scaled pose.

func unapplying(Pose3D) -> Rect3D

Returns a rectangle that results from unapplying the specified pose.

func unapplying(AffineTransform3D) -> Rect3D

Returns a rectangle that results from unapplying the specified affine transform.

### Checking characteristics

func contains(anyOf: [Point3D]) -> Bool

Returns a Boolean value that indicates whether the rectangle contains any of the specified points.

func intersects(Rect3D) -> Bool

Returns a Boolean value that indicates whether two rectangles intersect.

var isEmpty: Bool

A Boolean value that indicates whether two or three of the dimensions are zero.

### Creating derived 3D rectangles

var integral: Rect3D

Returns the smallest rectangle after converting the source rectangle values to integers.

func formInset(by: Size3D)

Insets the rectangle by the specified size.

func inset(by: Size3D) -> Rect3D

Returns a new rectangle with the same center point after applying the specified inset amount.

func intersection(Rect3D) -> Rect3D?

Returns the intersection of two rectangles.

var standardized: Rect3D

A rectangle with positive dimensions.

### Comparing values

static func == (Rect3D, Rect3D) -> Bool

Returns a Boolean value that indicates whether two values are equal.

### Applying arithmetic operations

static func * (AffineTransform3D, Rect3D) -> Rect3D

Returns the rectangle that results from applying the affine transform to the rectangle.

static func * (ProjectiveTransform3D, Rect3D) -> Rect3D

Returns the rectangle that results from applying the projective transform to the rectangle.

static func * (Pose3D, Rect3D) -> Rect3D

Returns a new rectangle after applying the pose to the rectangle.

### Deprecated symbols

func distance(to: Rect3D) -> Double

Returns the distance between the origins of two rectangle.

Deprecated

func containsAny(of: [Point3D]) -> Bool

Returns a Boolean value that indicates whether the rectangle contains any of the specified points.

Deprecated

func rotation(to: Rect3D) -> Rotation3D

Returns the rotation around @p (0,0,0) from the first rectangle to the second rectangle.

Deprecated

var maxX: DoubleDeprecated

var maxY: DoubleDeprecated

var maxZ: DoubleDeprecated

var midX: DoubleDeprecated

var midY: DoubleDeprecated

var midZ: DoubleDeprecated

var minX: DoubleDeprecated

var minY: DoubleDeprecated

var minZ: DoubleDeprecated

### Default Implementations

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
- Translatable3D
- Volumetric

## See Also

### 3D primitives

struct Point3D

A point in a 3D coordinate system.

struct Size3D

A size that describes width, height, and depth in a 3D coordinate system.

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

