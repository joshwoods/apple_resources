

- Spatial
- Ray3D
-  unapplying(\_:) 

Instance Method

# unapplying(\_:)

Unapplies the specified pose to the ray.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
func unapplying(_ pose: Pose3D) -> Ray3D
```

## Parameters 

`pose`  

The pose that the function unapplies to the ray.

## See Also

### Transforming a 3D ray structure

func apply(Pose3D)

Applies the specified pose to the ray.

func applying(AffineTransform3D) -> Ray3D

Returns a ray that results from applying the specified affine transform.

func applying(ProjectiveTransform3D) -> Ray3D

Returns a ray that results from applying the specified projective transform.

func applying(Pose3D) -> Ray3D

Returns a ray that results from applying the specified pose.

func unapplying(AffineTransform3D) -> Ray3D

Returns a ray that results from unapplying the specified affine transform.

func unapplying(ProjectiveTransform3D) -> Ray3D

Returns a ray that results from unapplying the specified projective transform.

func rotated(by: Rotation3D) -> Ray3D

Returns a ray that results from applying the specified rotation.

func rotated(by: simd_quatd) -> Ray3D

Returns a ray that results from rotating with the specified quaternion.

func rotated(by: simd_quatd, around: Point3D) -> Ray3D

Returns a ray that’s rotated by the specified quaternion around a specified pivot.

func rotated(by: Rotation3D, around: Point3D) -> Ray3D

Returns a ray that’s rotated by the specified rotation around a specified pivot.

func applying(ScaledPose3D) -> Ray3D

Returns a ray that’s transformed by the specified scaled pose.

func unapplying(ScaledPose3D) -> Ray3D

Returns a ray that’s transformed by the inverse of the specified scaled pose.

