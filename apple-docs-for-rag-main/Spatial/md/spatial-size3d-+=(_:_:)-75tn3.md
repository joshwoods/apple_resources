

- Spatial
- Size3D
-  +=(\_:\_:) 

Operator

# +=(\_:\_:)

Adds two size structures and stores the result in the left-hand-side variable.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
static func += (lhs: inout Size3D, rhs: Size3D)
```

## Parameters 

`lhs`  

The left-hand-side value.

`rhs`  

The right-hand-side value.

## See Also

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

