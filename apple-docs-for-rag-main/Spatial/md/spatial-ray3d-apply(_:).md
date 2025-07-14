

- Spatial
- Ray3D
-  apply(\_:) 

Instance Method

# apply(\_:)

Applies the specified pose to the ray.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
mutating func apply(_ pose: Pose3D)
```

## Parameters 

`pose`  

The pose that the function applies to the ray.

## See Also

### Transforming a 3D ray structure

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

func unapplying(Pose3D) -> Ray3D

Unapplies the specified pose to the ray.

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

