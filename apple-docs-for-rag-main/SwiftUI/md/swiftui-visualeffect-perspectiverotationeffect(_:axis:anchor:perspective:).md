

- SwiftUI
- VisualEffect
-  perspectiveRotationEffect(\_:axis:anchor:perspective:) 

Instance Method

# perspectiveRotationEffect(\_:axis:anchor:perspective:)

Renders content as if it’s rotated in three dimensions around the specified axis.

visionOS 1.0+

``` source
func perspectiveRotationEffect(
    _ angle: Angle,
    axis: (x: CGFloat, y: CGFloat, z: CGFloat),
    anchor: UnitPoint3D = .back,
    perspective: CGFloat = 1
) -> some VisualEffect
```

## Parameters 

`angle`  

The angle by which to rotate the content.

`axis`  

The axis of rotation, specified as a tuple with named elements for each of the three spatial dimensions.

`anchor`  

A unit point within the content about which to perform the rotation. The default value is center.

`perspective`  

The relative vanishing point for the rotation. The default is `1`.

## Return Value

A rotation effect.

## Discussion

Use this method to create the effect of rotating content in three dimensions around a specified axis of rotation. The modifier projects two dimensional content onto the original content’s plane. Use the `perspective` input to control the renderer’s vanishing point. The following example creates the appearance of rotating text 45˚ about the y-axis:

```
Text("Rotation by passing an angle in degrees")
    .visualEffect { content, geometryProxy in
        content
            .perspectiveRotationEffect(
                .degrees(45),
                axis: (x: 0.0, y: 1.0, z: 0.0),
                anchor: .center,
                perspective: 1)
        }
    .border(Color.gray)
```

Important

To truly rotate content in three dimensions, use a 3D rotation effect without a perspective input like rotation3DEffect(_:axis:anchor:).

## See Also

### Rotating

func rotationEffect(Angle, anchor: UnitPoint) -> some VisualEffect

Rotates content in two dimensions around the specified point.

func rotation3DEffect(Angle, axis: (x: CGFloat, y: CGFloat, z: CGFloat), anchor: UnitPoint, anchorZ: CGFloat, perspective: CGFloat) -> some VisualEffect

Renders content as if it’s rotated in three dimensions around the specified axis.

func rotation3DEffect(Rotation3D, anchor: UnitPoint3D) -> some VisualEffect

Rotates content by the specified 3D rotation value.

func rotation3DEffect(_:axis:anchor:)

Rotates content by an angle about an axis that you specify as a tuple of elements.

