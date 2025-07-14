

- SwiftUI
- VisualEffect
-  rotation3DEffect(\_:axis:anchor:) 

Instance Method

# rotation3DEffect(\_:axis:anchor:)

Rotates content by an angle about an axis that you specify as a tuple of elements.

visionOS 1.0+

``` source
func rotation3DEffect(
    _ angle: Angle,
    axis: (x: CGFloat, y: CGFloat, z: CGFloat), anchor: UnitPoint3D = .center
) -> some VisualEffect
```

Show all declarations

## Parameters 

`angle`  

The angle by which to rotate the content.

`axis`  

The axis of rotation, specified as a tuple with named elements for each of the three spatial dimensions.

`anchor`  

The unit point within the content about which to perform the rotation. The default value is center.

## Return Value

A rotation effect.

## Discussion

Note

During an animation, the angle and each element of the axis is interpolated separately, which may cause undesirable results. To achive more natual animations, cosinder using rotation3DEffect(_:anchor:)

This effect causes the content to appear rotated, but doesn’t change the content’s frame. The following code applies a rotation of 45° about the y-axis, using the default anchor point at the center of the content:

```
Model3D(named: "robot")
    .visualEffect { content, geometryProxy in
        content
            .rotation3DEffect(.degrees(45), axis: (x: 0, y: 1, z: 0))
    }
```

Note

The following example is not equivalent to the previous. This example will use spherical linear interpolation during an animation.

```
Model3D(named: "robot")
    .rotation3DEffect(Rotation3D(.init(degrees: 45), axis: .y)
```

## See Also

### Rotating

func rotationEffect(Angle, anchor: UnitPoint) -> some VisualEffect

Rotates content in two dimensions around the specified point.

func rotation3DEffect(Angle, axis: (x: CGFloat, y: CGFloat, z: CGFloat), anchor: UnitPoint, anchorZ: CGFloat, perspective: CGFloat) -> some VisualEffect

Renders content as if it’s rotated in three dimensions around the specified axis.

func perspectiveRotationEffect(Angle, axis: (x: CGFloat, y: CGFloat, z: CGFloat), anchor: UnitPoint3D, perspective: CGFloat) -> some VisualEffect

Renders content as if it’s rotated in three dimensions around the specified axis.

func rotation3DEffect(Rotation3D, anchor: UnitPoint3D) -> some VisualEffect

Rotates content by the specified 3D rotation value.

