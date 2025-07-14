

- RealityKit
- Model3D
-  rotation3DEffect(\_:axis:anchor:) 

Instance Method

# rotation3DEffect(\_:axis:anchor:)

Rotates the view’s content by an angle about an axis that you specify as a tuple of elements.

RealityKitSwiftUIvisionOS 1.0+

``` source
nonisolated
func rotation3DEffect(
    _ angle: Angle,
    axis: (x: CGFloat, y: CGFloat, z: CGFloat),
    anchor: UnitPoint3D = .center
) -> some View
```

## Parameters 

`angle`  

The angle by which to rotate the view’s content.

`axis`  

The axis of rotation, specified as a tuple with named elements for each of the three spatial dimensions.

`anchor`  

The unit point within the view about which to perform the rotation. The default value is `UnitPoint3D/center`.

## Return Value

A view with rotated content.

## Discussion

Note

During an animation, the angle and each element of the axis is interpolated separately, which may cause undesirable results. To achive more natual animations, cosinder using `View/rotation3DEffect(_:anchor:)`

This modifier rotates the view’s content without changing the view’s frame. The following code displays a 3D model with a rotation of 45° about the y-axis using the default anchor point at the center of the view:

```
Model3D(named: "robot")
    .rotation3DEffect(.degrees(45), axis: (x: 0, y: 1, z: 0))
```

Note

The following example is not equivalent to the previous. This example will use spherical linear interpolation during an animation.

```
let rotation = Rotation3D(
    .init(degrees: 45), axis: RotationAxis3D(x: 0, y: 1, z: 0))
Model3D(named: "robot")
    .rotation3DEffect(rotation)
```

