

- Foundation
-  AffineTransform 

Structure

# AffineTransform

A graphics coordinate transformation.

iOS 8.0+iPadOS 8.0+macOS 10.10+tvOS 9.0+watchOS 2.0+

``` source
struct AffineTransform
```

## Topics

### Creating Transforms

init()

Creates an affine transformation matrix with identity values.

init(rotationByDegrees: CGFloat)

Creates an affine transformation matrix from a rotation angle.

init(rotationByRadians: CGFloat)

Creates an affine transformation matrix from a rotation angle.

init(scale: CGFloat)

Creates an affine transformation matrix from scaling a single value.

init(scaleByX: CGFloat, byY: CGFloat)

Creates an affine transformation matrix from scaling values.

init(translationByX: CGFloat, byY: CGFloat)

Creates an affine transformation matrix from translation values.

init(m11: CGFloat, m12: CGFloat, m21: CGFloat, m22: CGFloat, tX: CGFloat, tY: CGFloat)

Creates an affine transformation.

### Getting the Identity Transform

static let identity: AffineTransform

An identity affine transformation matrix.

### Accumulating Tranformations

func rotate(byDegrees: CGFloat)

Mutates an affine transformation matrix to apply a rotation.

func rotate(byRadians: CGFloat)

Mutates an affine transformation matrix to apply a rotation.

func scale(CGFloat)

Mutates an affine transformation matrix to apply scaling in both x and y dimensions.

func scale(x: CGFloat, y: CGFloat)

Mutates an affine transformation matrix to apply scaling in each of the x and y dimensions.

func translate(x: CGFloat, y: CGFloat)

Mutates an affine transformation matrix to perform the specified translation.

func append(AffineTransform)

Mutates an affine transformation by appending another affine transform.

func prepend(AffineTransform)

Mutates an affine transformation by prepending another affine transform.

func invert()

Inverts the transformation matrix, if possible.

func inverted() -> AffineTransform?

Returns an inverted version of the matrix, if possible, or nil if not.

### Transforming Data and Objects

func transform(NSPoint) -> NSPoint

Applies the affine transform to the specified point.

func transform(NSSize) -> NSSize

Applies the affine transform to the specified size.

### Accessing the Transformation Matrix

var m11: CGFloat

An element of the transform matrix that contributes scaling, rotation, and shear.

var m12: CGFloat

An element of the transform matrix that contributes scaling, rotation, and shear.

var m21: CGFloat

An element of the transform matrix that contributes scaling, rotation, and shear.

var m22: CGFloat

An element of the transform matrix that contributes scaling, rotation, and shear.

var tX: CGFloat

An element of the transform matrix that contributes translation.

var tY: CGFloat

An element of the transform matrix that contributes translation.

### Using Reference Types

class NSAffineTransform

A graphics coordinate transformation.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- ReferenceConvertible
- Sendable

## See Also

### Geometry

@frozen struct CGFloat

The basic type for floating-point scalar values in Core Graphics and related frameworks.

typealias NSPoint

A point in a Cartesian coordinate system.

typealias NSSize

A two-dimensional size.

typealias NSRect

A rectangle.

struct NSEdgeInsets

A description of the distance between the edges of two rectangles.

