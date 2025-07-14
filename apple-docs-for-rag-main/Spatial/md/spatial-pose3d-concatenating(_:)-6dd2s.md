

- Spatial
- Pose3D
-  concatenating(\_:) 

Instance Method

# concatenating(\_:)

Returns a pose that represents the concatenation of two poses.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func concatenating(_ transform: Pose3D) -> Pose3D
```

## Parameters 

`transform`  

The second pose.

## See Also

### Transforming a 3D pose structure

func concatenating(ScaledPose3D) -> ScaledPose3D

Returns a pose that represents the concatenation of a scaled pose and a pose.

func flip(along: Axis3D)

Flips a pose along the specified axis.

func flipped(along: Axis3D) -> Pose3D

Returns a pose that results from flipping it along the specified axis.

func rotated(by: simd_quatd) -> Pose3D

Returns a pose that results from rotating with the specified quaternion.

func rotated(by: Rotation3D) -> Pose3D

Returns a pose that results from applying the specified rotation.

