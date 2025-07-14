

- Spatial
- Rect3D
-  \*(\_:\_:) 

Operator

# \*(\_:\_:)

Returns the rectangle that results from applying the projective transform to the rectangle.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
static func * (lhs: ProjectiveTransform3D, rhs: Rect3D) -> Rect3D
```

## Parameters 

`lhs`  

The left-hand-side value.

`rhs`  

The right-hand-side value.

## See Also

### Applying arithmetic operations

static func * (AffineTransform3D, Rect3D) -> Rect3D

Returns the rectangle that results from applying the affine transform to the rectangle.

static func * (Pose3D, Rect3D) -> Rect3D

Returns a new rectangle after applying the pose to the rectangle.

