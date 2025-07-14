

- Spatial
- Rect3D
-  rotated(by:around:) 

Instance Method

# rotated(by:around:)

Returns a rectangle that results from applying the specified rotation around a pivot point.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func rotated(
    by rotation: Rotation3D,
    around pivot: Point3D
) -> Rect3D
```

## Parameters 

`rotation`  

The rotation structure that defines the rotation’s angle and axis.

`pivot`  

The point structure that defines the rotation pivot point.

## Return Value

The rectangle that results from applying the specified rotation around a pivot point.

## See Also

### Transforming a 3D rectangle structure

func applying(Pose3D) -> Rect3D

Returns a rectangle that results from applying the specified pose.

func applying(ScaledPose3D) -> Rect3D

Returns a rectangle that’s transformed by the specified scaled pose.

func applying(ScaledPose3D) -> Rect3D

Returns a rectangle that’s transformed by the specified scaled pose.

func rotated(by: simd_quatd, around: Point3D) -> Rect3D

Returns a rectangle that results from rotating with the specified quaternion around a pivot point.

func scaledBy(x: Double, y: Double, z: Double) -> Rect3D

Returns a rectangle that results from scaling with the specified double-precision values.

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

