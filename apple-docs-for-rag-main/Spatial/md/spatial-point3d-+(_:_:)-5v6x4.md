

- Spatial
- Point3D
-  +(\_:\_:) 

Operator

# +(\_:\_:)

Returns a point that’s the element-wise sum of a point and a size.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
static func + (lhs: Point3D, rhs: Size3D) -> Point3D
```

## Parameters 

`lhs`  

The left-hand-side value.

`rhs`  

The right-hand-side value.

## See Also

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

