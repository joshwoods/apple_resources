

- Spatial
- Rotation3D
-  swingTwist(twistAxis:) 

Instance Method

# swingTwist(twistAxis:)

Returns the rotation’s swing-twist decomposition for a given twist axis.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
func swingTwist(twistAxis: RotationAxis3D) -> (swing: Rotation3D, twist: Rotation3D)
```

## Parameters 

`twistAxis`  

The twist axis.

## Return Value

A tuple that contains the swing rotation and the twist rotation.

## See Also

### Decomposing a 3D rotation structure

func swing(twistAxis: RotationAxis3D) -> Rotation3D

Returns the swing component of the rotation’s swing-twist decomposition for a given twist axis.

func twist(twistAxis: RotationAxis3D) -> Rotation3D

Returns the twist component of the rotation’s swing-twist decomposition for a given twist axis.

func swing(twistAxis: RotationAxis3D) -> Rotation3D

Returns the swing component of the rotation’s swing-twist decomposition for a given twist axis.

func twist(twistAxis: RotationAxis3D) -> Rotation3D

Returns the twist component of the rotation’s swing-twist decomposition for a given twist axis.

