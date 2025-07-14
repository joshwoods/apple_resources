

- Spatial
-  ProjectiveTransform3D 

Structure

# ProjectiveTransform3D

A 3D projective transformation matrix.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct ProjectiveTransform3D
```

## Topics

### Creating a 3D projective transform structure

init()

Creates a projective transform.

init()

Returns a new identity projective transform.

init(simd_float4x4)

Creates a projective transform from the specified 4 x 4 single-precision matrix.

init(simd_double4x4)

Creates a projective transform from the specified double-precision matrix.

init(matrix: simd_double4x4)

Creates a projective transform from the specified 4 x 4 double-precision matrix.

init(AffineTransform3D)

Creates a projective transform from the specified affine transform.

init(pose: Pose3D)

Creates a projective transform from the specified pose structure.

init(scale: Size3D, rotation: Rotation3D, translation: Vector3D)

Creates a projective transform from the specified scale, rotate, and translate transforms.

init(scale: Size3D)

Creates a projective transform from the specified scale transform.

init(rotation: Rotation3D)

Creates a projective transform from the specified rotate transform.

init(translation: Vector3D)

Creates a projective transform from the specified translate transform.

init(shear: AxisWithFactors)

Creates a projective transform from the specified shear transform.

init(leftTangent: Double, rightTangent: Double, topTangent: Double, bottomTangent: Double, nearZ: Double, farZ: Double, reverseZ: Bool)

Returns a projective transform from tangents for each side of its frustum.

init(fovY: Angle2D, aspectRatio: Double, nearZ: Double, farZ: Double)

Returns a projective transform with right-hand side perspective.

init(fovY: Angle2D, aspectRatio: Double, nearZ: Double, farZ: Double, reverseZ: Bool)

init(scaledPose: ScaledPose3D)

### Inspecting a 3D projective transform’s properties

var inverse: ProjectiveTransform3D?

The projective transform’s inverse.

var scaleComponent: Size3D

The scale component of the projective transform.

var translation: Vector3D

The translation component of the projective transform.

var matrix: simd_double4x4

The projective transform’s underlying matrix.

static let identity: ProjectiveTransform3D

The identity transform.

### Transforming a 3D projective transform structure

func sheared(AxisWithFactors) -> ProjectiveTransform3D

Returns a projective transform that results from shearing over an axis by shear factors for the other two axes.

enum AxisWithFactors

Constants that describe the axis of a shear transform.

struct Axis3D

Constants that describe an axis.

func concatenating(ProjectiveTransform3D) -> ProjectiveTransform3D

Returns a projective transformation matrix that results from concatenating two existing projective transforms.

func flip(along: Axis3D)

Flips a projective transform along the specified axis.

func flipped(along: Axis3D) -> ProjectiveTransform3D

Returns a projective transform that results from flipping it along the specified axis.

### Decomposing a 3D projective transform

var rotation: Rotation3D?

The projective transform’s rotation.

### Checking characteristics

func is3DProjection() -> Bool

Returns a Boolean value that indicates whether the transform is a 3D projection.

func isUniform(overDimensions: Dimension3DSet) -> Bool

Returns a Boolean value that indicates whether the transform scales equally over the specified dimensions.

var isAffine: Bool

A Boolean value that indicates whether the transform is affine.

var isIdentity: Bool

A Boolean value that indicates whether the transform is the identity transform.

var isRectilinear: Bool

A Boolean value that indicates whether the transform is rectilinear.

var isTranslation: Bool

A Boolean value that indicates whether the transform contains only a translation.

var isUniform: Bool

A Boolean value that indicates whether the transform scales equally over all dimensions.

var isInvertible: Bool

Returns a Boolean value that indicates whether the transform is invertible.

### Comparing values

func isApproximatelyEqual(to: ProjectiveTransform3D, tolerance: Double) -> Bool

Returns a Boolean value that indicates whether two transforms are equal within a specified tolerance.

### Applying arithmetic operations

static func * (ProjectiveTransform3D, ProjectiveTransform3D) -> ProjectiveTransform3D

Returns the concatenation of two projective transforms.

static func *= (inout ProjectiveTransform3D, ProjectiveTransform3D)

Concatenates two projective transforms and stores the result in the left-hand-side variable.

### Deprecated symbols

var offset: Vector3D

The projective transform’s translation.

Deprecated

var scale: Size3D?

The projective transform’s scale.

Deprecated

func inverted() -> ProjectiveTransform3D?

Returns a new transform that results from inverting an existing projective transform.

Deprecated

init(matrix: simd_float4x4)

Creates a projective transform from the specified 4 x 4 single-precision matrix.

Deprecated

init(scale: Size3D, rotation: Rotation3D, translation: Size3D)

Creates a projective transform from the specified scale, rotate, and translate transforms.

Deprecated

init(fovyRadians: Double, aspectRatio: Double, nearZ: Double, farZ: Double, reverseZ: Bool)

Returns a projective transform with right-hand-side perspective and optional reverse-z.

Deprecated

init(translation: Size3D)Deprecated

init(fovyRadians: Double, aspectRatio: Double, nearZ: Double, farZ: Double)Deprecated

### Default Implementations

CustomReflectable Implementations

Scalable3D Implementations

Shearable3D Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- CustomReflectable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Rotatable3D
- Scalable3D
- Sendable
- Shearable3D
- Translatable3D

## See Also

### Affine and projective transforms

struct AffineTransform3D

A 3D affine transformation matrix.

