

- Spatial
- AffineTransform3D
-  isUniform(overDimensions:) 

Instance Method

# isUniform(overDimensions:)

Returns a Boolean value that indicates whether the transform scales equally over the specified dimensions.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func isUniform(overDimensions: Dimension3DSet) -> Bool
```

## Parameters 

`overDimensions`  

The dimensions that the function checks over.

## Return Value

A Boolean value that indicates whether the transform scales equally over the specified dimensions.

## See Also

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

var isUniform: Bool

A Boolean value that indicates whether the transform scales equally over all dimensions.

var matrix: simd_double4x3

The affine transform’s underlying matrix.

var matrix3x3: simd_double3x3

The first three columns of an affine transform’s underlying matrix.

var matrix4x4: simd_double4x4

A 4 x 4 matrix that results from constructing the affine transform’s underlying matrix.

