

- Spatial
-  Dimension3DSet 

Structure

# Dimension3DSet

A set of dimensions.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
struct Dimension3DSet
```

## Topics

### Type properties

static let all: Dimension3DSet

All dimensions.

static let x: Dimension3DSet

The x-dimension.

static let y: Dimension3DSet

The y-dimension.

static let z: Dimension3DSet

The z-dimension.

### Instance properties

let rawValue: Int

The corresponding value of the raw type.

### Initializers

init(rawValue: Int)

Creates a new instance with the specified raw value.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

## See Also

### Checking characteristics

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

