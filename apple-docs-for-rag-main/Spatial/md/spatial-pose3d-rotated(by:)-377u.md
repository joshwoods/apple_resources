

- Spatial
- Pose3D
-  rotated(by:) 

Instance Method

# rotated(by:)

Returns a pose that results from applying the specified rotation.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func rotated(by rotation: Rotation3D) -> Pose3D
```

## Parameters 

`rotation`  

The rotation structure that defines the rotation’s angle and axis.

## See Also

### Transforming a 3D pose structure

func concatenating(ScaledPose3D) -> ScaledPose3D

Returns a pose that represents the concatenation of a scaled pose and a pose.

func concatenating(Pose3D) -> Pose3D

Returns a pose that represents the concatenation of two poses.

func flip(along: Axis3D)

Flips a pose along the specified axis.

func flipped(along: Axis3D) -> Pose3D

Returns a pose that results from flipping it along the specified axis.

func rotated(by: simd_quatd) -> Pose3D

Returns a pose that results from rotating with the specified quaternion.

