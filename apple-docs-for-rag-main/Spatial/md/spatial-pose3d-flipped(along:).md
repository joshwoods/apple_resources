

- Spatial
- Pose3D
-  flipped(along:) 

Instance Method

# flipped(along:)

Returns a pose that results from flipping it along the specified axis.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func flipped(along axis: Axis3D) -> Pose3D
```

## Parameters 

`axis`  

An axis structure that specifies the flip axis.

## See Also

### Transforming a 3D pose structure

func concatenating(ScaledPose3D) -> ScaledPose3D

Returns a pose that represents the concatenation of a scaled pose and a pose.

func concatenating(Pose3D) -> Pose3D

Returns a pose that represents the concatenation of two poses.

func flip(along: Axis3D)

Flips a pose along the specified axis.

func rotated(by: simd_quatd) -> Pose3D

Returns a pose that results from rotating with the specified quaternion.

func rotated(by: Rotation3D) -> Pose3D

Returns a pose that results from applying the specified rotation.

