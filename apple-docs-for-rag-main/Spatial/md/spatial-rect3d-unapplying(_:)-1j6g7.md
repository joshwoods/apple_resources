

- Spatial
- Rect3D
-  unapplying(\_:) 

Instance Method

# unapplying(\_:)

Returns a rectangle that results from unapplying the specified projective transform.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func unapplying(_ transform: ProjectiveTransform3D) -> Rect3D
```

## Parameters 

`transform`  

The projective transform that the function unapplies to the rectangle.

## Return Value

The rectangle that results from unapplying the specified projective transform.

## See Also

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

func unapplying(ScaledPose3D) -> Rect3D

Returns a rectangle that’s transformed by the inverse of the specified scaled pose.

func unapplying(Pose3D) -> Rect3D

Returns a rectangle that results from unapplying the specified pose.

func unapplying(AffineTransform3D) -> Rect3D

Returns a rectangle that results from unapplying the specified affine transform.

