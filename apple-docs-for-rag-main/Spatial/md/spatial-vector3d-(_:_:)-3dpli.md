

- Spatial
- Vector3D
-  \*(\_:\_:) 

Operator

# \*(\_:\_:)

Returns the vector that results from applying the projective transform to the vector.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
static func * (lhs: ProjectiveTransform3D, rhs: Vector3D) -> Vector3D
```

## Parameters 

`lhs`  

The left-hand-side value.

`rhs`  

The right-hand-side value.

## See Also

### Applying arithmetic operations

static func * (Vector3D, Double) -> Vector3D

Returns a vector that’s the product of a vector and a scalar value.

static func * (Double, Vector3D) -> Vector3D

Returns a vector that’s the product of a scalar value and a vector.

static func * (AffineTransform3D, Vector3D) -> Vector3D

Returns the vector that results from applying the affine transform to the vector.

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

