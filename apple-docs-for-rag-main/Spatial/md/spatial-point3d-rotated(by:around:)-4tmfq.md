

- Spatial
- Point3D
-  rotated(by:around:) 

Instance Method

# rotated(by:around:)

Returns a point that results from applying a rotation around the specified point.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func rotated(
    by rotation: Rotation3D,
    around pivot: Point3D
) -> Point3D
```

## Parameters 

`rotation`  

A point that defines the rotation pivot.

`pivot`  

The rotation structure that defines the rotation’s angle and axis.

## Return Value

The point that results from applying the specified rotation.

## See Also

### Transforming a 3D point structure

func applying(ScaledPose3D) -> Point3D

Returns a point that’s transformed by the specified scaled pose.

func applying(ScaledPose3D) -> Point3D

Returns a point that’s transformed by the specified scaled pose.

func applying(Pose3D) -> Point3D

Returns a point that results from applying the specified pose.

func clamp(to: Rect3D)

Clamps the mutable point to the specified rectangle.

func clamped(to: Rect3D) -> Point3D

Returns a point with coordinates that clamp to the specified rectangle.

func scale(by: Double)

func rotated(by: simd_quatd, around: Point3D) -> Point3D

Returns a point that results from rotating with a quaternion around the specified point.

func unapplying(Pose3D) -> Point3D

Returns a point that results from unapplying the specified pose.

func unapplying(ScaledPose3D) -> Point3D

Returns a point that’s transformed by the inverse of the specified scaled pose.

func unapplying(ScaledPose3D) -> Point3D

Returns a point that’s transformed by the inverse of the specified scaled pose.

