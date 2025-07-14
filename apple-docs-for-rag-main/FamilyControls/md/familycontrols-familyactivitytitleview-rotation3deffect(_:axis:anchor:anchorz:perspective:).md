

- FamilyControls
- FamilyActivityTitleView
-  rotation3DEffect(\_:axis:anchor:anchorZ:perspective:) 

Instance Method

# rotation3DEffect(\_:axis:anchor:anchorZ:perspective:)

Renders a view’s content as if it’s rotated in three dimensions around the specified axis.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func rotation3DEffect(
    _ angle: Angle,
    axis: (x: CGFloat, y: CGFloat, z: CGFloat),
    anchor: UnitPoint = .center,
    anchorZ: CGFloat = 0,
    perspective: CGFloat = 1
) -> some View
```

## Parameters 

`angle`  

The angle by which to rotate the view’s content.

`axis`  

The axis of rotation, specified as a tuple with named elements for each of the three spatial dimensions.

`anchor`  

A two dimensional unit point within the view about which to perform the rotation. The default value is `UnitPoint/center`.

`anchorZ`  

The location on the z-axis around which to rotate the content. The default is `0`.

`perspective`  

The relative vanishing point for the rotation. The default is `1`.

## Return Value

A view with rotated content.

## Discussion

Use this method to create the effect of rotating a view in three dimensions around a specified axis of rotation. The modifier projects the rotated content onto the original view’s plane. Use the `perspective` value to control the renderer’s vanishing point. The following example creates the appearance of rotating text 45˚ about the y-axis:

```
Text("Rotation by passing an angle in degrees")
    .rotation3DEffect(
        .degrees(45),
        axis: (x: 0.0, y: 1.0, z: 0.0),
        anchor: .center,
        anchorZ: 0,
        perspective: 1)
    .border(Color.gray)
```

Important

In visionOS, create this effect with `perspectiveRotationEffect(_:axis:anchor:anchorZ:perspective:)` instead. To truly rotate a view in three dimensions, use a 3D rotation modifier without a perspective input like `rotation3DEffect(_:axis:anchor:)`.

