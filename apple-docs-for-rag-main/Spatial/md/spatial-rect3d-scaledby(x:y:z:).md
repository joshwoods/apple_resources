

- Spatial
- Rect3D
-  scaledBy(x:y:z:) 

Instance Method

# scaledBy(x:y:z:)

Returns a rectangle that results from scaling with the specified double-precision values.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func scaledBy(
    x: Double = 1,
    y: Double = 1,
    z: Double = 1
) -> Rect3D
```

## Parameters 

`x`  

The double-precision value that specifies the scale along the x-dimension.

`y`  

The double-precision value that specifies the scale along the y-dimension.

`z`  

The double-precision value that specifies the scale along the z-dimension.

## Return Value

The rectangle that results from scaling with the specified double-precision values.

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

func sheared(AxisWithFactors) -> Rect3D

Returns a rectangle that results from shearing over an axis by shear factors for the other two axes.

func unapplying(ProjectiveTransform3D) -> Rect3D

Returns a rectangle that results from unapplying the specified projective transform.

func unapplying(ScaledPose3D) -> Rect3D

Returns a rectangle that’s transformed by the inverse of the specified scaled pose.

func unapplying(Pose3D) -> Rect3D

Returns a rectangle that results from unapplying the specified pose.

func unapplying(AffineTransform3D) -> Rect3D

Returns a rectangle that results from unapplying the specified affine transform.

