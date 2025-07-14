

- Spatial
- Point3D
-  clamp(to:) 

Instance Method

# clamp(to:)

Clamps the mutable point to the specified rectangle.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
mutating func clamp(to rect: Rect3D)
```

## Parameters 

`rect`  

The rectangle structure that defines the clamp volume.

## See Also

### Transforming a 3D point structure

func applying(ScaledPose3D) -> Point3D

Returns a point that’s transformed by the specified scaled pose.

func applying(ScaledPose3D) -> Point3D

Returns a point that’s transformed by the specified scaled pose.

func applying(Pose3D) -> Point3D

Returns a point that results from applying the specified pose.

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

