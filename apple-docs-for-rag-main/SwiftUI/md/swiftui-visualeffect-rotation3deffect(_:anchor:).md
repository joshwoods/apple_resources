

- SwiftUI
- VisualEffect
-  rotation3DEffect(\_:anchor:) 

Instance Method

# rotation3DEffect(\_:anchor:)

Rotates content by the specified 3D rotation value.

visionOS 1.0+

``` source
func rotation3DEffect(
    _ rotation: Rotation3D,
    anchor: UnitPoint3D = .center
) -> some VisualEffect
```

## Parameters 

`rotation`  

A rotation to apply to the content.

`anchor`  

The unit point within the content about which to perform the rotation. The default value is center.

## Return Value

A rotation effect.

## Discussion

This effect causes the content to appear rotated, but doesn’t change the content’s frame. The following code applies a rotation of 45° about the y-axis, using the default anchor point at the center of the content:

```
Model3D(named: "robot")
    .visualEffect { content, geometryProxy in
        content
            .rotation3DEffect(Rotation3D(angle: .degrees(45), axis: .y))
    }
```

During an animation, this modifier uses spherical linear interpolation, which produces more natural animations, but doesn’t support rotations over 360 degrees. To specify angles over 360 degrees, consider using `View/rotation3DEffect(_:axis:anchor:)-4enag`.

## See Also

### Rotating

func rotationEffect(Angle, anchor: UnitPoint) -> some VisualEffect

Rotates content in two dimensions around the specified point.

func rotation3DEffect(Angle, axis: (x: CGFloat, y: CGFloat, z: CGFloat), anchor: UnitPoint, anchorZ: CGFloat, perspective: CGFloat) -> some VisualEffect

Renders content as if it’s rotated in three dimensions around the specified axis.

func perspectiveRotationEffect(Angle, axis: (x: CGFloat, y: CGFloat, z: CGFloat), anchor: UnitPoint3D, perspective: CGFloat) -> some VisualEffect

Renders content as if it’s rotated in three dimensions around the specified axis.

func rotation3DEffect(_:axis:anchor:)

Rotates content by an angle about an axis that you specify as a tuple of elements.

