

- Spatial
- Point3D
-  applying(\_:) 

Instance Method

# applying(\_:)

Returns a point that results from applying the specified pose.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func applying(_ pose: Pose3D) -> Point3D
```

## Parameters 

`pose`  

The pose that the function applies to the point.

## See Also

### Transforming a 3D point structure

func applying(ScaledPose3D) -> Point3D

Returns a point that’s transformed by the specified scaled pose.

func applying(ScaledPose3D) -> Point3D

Returns a point that’s transformed by the specified scaled pose.

func clamp(to: Rect3D)

Clamps the mutable point to the specified rectangle.

func clamped(to: Rect3D) -> Point3D

Returns a point with coordinates that clamp to the specified rectangle.

func scale(by: Double)

func rotated(by: Rotation3D, around: Point3D) -> Point3D

Returns a point that results from applying a rotation around the specified point.

func rotated(by: simd_quatd, around: Point3D) -> Point3D

Returns a point that results from rotating with a quaternion around the specified point.

func unapplying(Pose3D) -> Point3D

Returns a point that results from unapplying the specified pose.

func unapplying(ScaledPose3D) -> Point3D

Returns a point that’s transformed by the inverse of the specified scaled pose.

func unapplying(ScaledPose3D) -> Point3D

Returns a point that’s transformed by the inverse of the specified scaled pose.

