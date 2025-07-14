

- Spatial
- Rotation3D
-  twist(twistAxis:) 

Instance Method

# twist(twistAxis:)

Returns the twist component of the rotation’s swing-twist decomposition for a given twist axis.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func twist(twistAxis: RotationAxis3D) -> Rotation3D
```

## Parameters 

`twistAxis`  

The twist axis.

## Return Value

The twist component of the rotation’s swing-twist decomposition for a given twist axis.

## See Also

### Decomposing a 3D rotation structure

func swing(twistAxis: RotationAxis3D) -> Rotation3D

Returns the swing component of the rotation’s swing-twist decomposition for a given twist axis.

func swingTwist(twistAxis: RotationAxis3D) -> (swing: Rotation3D, twist: Rotation3D)

Returns the rotation’s swing-twist decomposition for a given twist axis.

func swing(twistAxis: RotationAxis3D) -> Rotation3D

Returns the swing component of the rotation’s swing-twist decomposition for a given twist axis.

