

- Spatial
-  AffineTransform3D 

Structure

# AffineTransform3D

A 3D affine transformation matrix.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct AffineTransform3D
```

## Topics

### Creating a 3D affine transform structure

init()

Creates an affine transform.

init()

Returns a new identity affine transform.

init(simd_float4x3)

Creates an affine transform from the specified single-precision matrix.

init(simd_double4x3)

Creates an affine transform from the specified 4 x 3 double-precision matrix.

init(Transform)

Creates an affine transform from the specified transform.

init(matrix: simd_double4x3)

Creates an affine transform from the specified double-precision matrix.

init(pose: Pose3D)

Creates an affine transform from the specified pose structure.

init(rotation: Rotation3D)

Creates an affine transform from the specified rotate transform.

init(scale: Size3D)

Creates an affine transform from the specified scale transform.

init(scale: Size3D, rotation: Rotation3D, translation: Vector3D)

Creates an affine transform from the specified scale, rotate, and translate transforms.

init(scaledPose: ScaledPose3D)

Creates an affine transform from the specified scale pose structure.

init(shear: AxisWithFactors)

Creates an affine transform from the specified shear transform.

init(translation: Vector3D)

Creates an affine transform from the specified translate transform.

init(truncating: ProjectiveTransform3D)

Returns a new affine transform structure from the specified projective transform.

init(truncating: simd_float4x4)

Returns a new affine transform structure from the specified single-precision 4 x 4 matrix truncated to a 4 x 3 matrix.

init(truncating: simd_double4x4)

Returns a new affine transform structure from the specified 4 x 4 matrix truncated to a 4 x 3 matrix.

### Transforming a 3D affine transform structure

struct Axis3D

Constants that describe an axis.

enum AxisWithFactors

Constants that describe the axis of a shear transform.

func changeBasis(from: AffineTransform3D, to: AffineTransform3D) -> AffineTransform3D?

Returns a new affine transform structure by applying a change-of-basis.

func concatenating(AffineTransform3D) -> AffineTransform3D

Returns an affine transformation matrix that results from concatenating two existing affine transforms.

func flip(along: Axis3D)

Flips an affine transform along the specified axis.

func flipped(along: Axis3D) -> AffineTransform3D

Returns an affine transform that results from flipping it along the specified axis.

var inverse: AffineTransform3D?

The affine transform’s inverse.

func scaledBy(x: Double, y: Double, z: Double) -> AffineTransform3D

Returns a transform that results from scaling with specified double-precision values.

func sheared(AxisWithFactors) -> AffineTransform3D

Returns an affine transform that results from shearing over an axis by shear factors for the other two axes.

### Decomposing a 3D affine transform

static let identity: AffineTransform3D

The identity transform.

var rotation: Rotation3D?

The affine transform’s rotation.

var scale: Size3D

The affine transform’s scale.

var translation: Vector3D

The translation component of the affine transform.

### Checking characteristics

struct Dimension3DSet

A set of dimensions.

var isIdentity: Bool

A Boolean value that indicates whether the transform is the identity transform.

var isInvertible: Bool

Returns a Boolean value that indicates whether the transform is invertible.

var isRectilinear: Bool

A Boolean value that indicates whether the transform is rectilinear.

var isTranslation: Bool

A Boolean value that indicates whether the transform contains only a translation.

func isUniform(overDimensions: Dimension3DSet) -> Bool

Returns a Boolean value that indicates whether the transform scales equally over the specified dimensions.

var isUniform: Bool

A Boolean value that indicates whether the transform scales equally over all dimensions.

var matrix: simd_double4x3

The affine transform’s underlying matrix.

var matrix3x3: simd_double3x3

The first three columns of an affine transform’s underlying matrix.

var matrix4x4: simd_double4x4

A 4 x 4 matrix that results from constructing the affine transform’s underlying matrix.

### Comparing values

static func == (AffineTransform3D, AffineTransform3D) -> Bool

Returns a Boolean value that indicates whether two values are equal.

func isApproximatelyEqual(to: AffineTransform3D, tolerance: Double) -> Bool

Returns a Boolean value that indicates whether two transforms are equal within a specified tolerance.

### Applying arithmetic operations

static func * (AffineTransform3D, AffineTransform3D) -> AffineTransform3D

Returns the concatenation of two affine transforms.

static func *= (inout AffineTransform3D, AffineTransform3D)

Concatenates two affine transforms and stores the result in the left-hand-side variable.

### Deprecated symbols

init?(simd_float4x4)

Creates an affine transform from the specified 4 x 4 single-precision matrix.

Deprecated

init?(simd_double4x4)

Creates an affine transform from the specified 4 x 4 double-precision matrix.

Deprecated

init?(matrix: simd_double4x4)

Creates an affine transform from the specified 4 x 4 double-precision matrix.

Deprecated

init(matrix: simd_float4x3)

Creates an affine transform from the specified single-precision matrix.

Deprecated

init?(matrix: simd_float4x4)

Creates an affine transform from the specified 4 x 4 single-precision matrix.

Deprecated

init?(projectiveTransform: ProjectiveTransform3D)

Creates an affine transform from the specified projective transform.

Deprecated

init(scale: Size3D, rotation: Rotation3D, translation: Size3D)

Creates an affine transform from the specified scale, rotate, and translate transforms.

Deprecated

init(translation: Size3D)Deprecated

func inverted() -> AffineTransform3D?

Returns a new transform that results from inverting an existing affine transform.

Deprecated

var offset: Vector3D

The affine transform’s translation.

Deprecated

### Default Implementations

CustomReflectable Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

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

struct ProjectiveTransform3D

A 3D projective transformation matrix.

