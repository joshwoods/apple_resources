

- FamilyControls
- FamilyActivityPicker
-  rotationEffect(\_:anchor:) 

Instance Method

# rotationEffect(\_:anchor:)

Rotates a view’s rendered output in two dimensions around the specified point.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func rotationEffect(
    _ angle: Angle,
    anchor: UnitPoint = .center
) -> some View
```

## Parameters 

`angle`  

The angle by which to rotate the view.

`anchor`  

A unit point within the view about which to perform the rotation. The default value is `UnitPoint/center`.

## Return Value

A view with rotated content.

## Discussion

This modifier rotates the view’s content around the axis that points out of the xy-plane. It has no effect on the view’s frame. The following code rotates text by 22˚ and then draws a border around the modified view to show that the frame remains unchanged by the rotation modifier:

```
Text("Rotation by passing an angle in degrees")
    .rotationEffect(.degrees(22))
    .border(Color.gray)
```

## See Also

### Rotation and Transformation

func rotation3DEffect(Angle, axis: (x: CGFloat, y: CGFloat, z: CGFloat), anchor: UnitPoint, anchorZ: CGFloat, perspective: CGFloat) -> some View

Renders a view’s content as if it’s rotated in three dimensions around the specified axis.

func projectionEffect(ProjectionTransform) -> some View

Applies a projection transformation to this view’s rendered output.

func transformEffect(CGAffineTransform) -> some View

Applies an affine transformation to this view’s rendered output.

