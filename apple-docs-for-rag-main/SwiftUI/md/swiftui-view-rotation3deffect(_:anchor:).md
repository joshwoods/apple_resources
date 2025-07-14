

- SwiftUI
- View
-  rotation3DEffect(\_:anchor:) 

Instance Method

# rotation3DEffect(\_:anchor:)

Rotates the view’s content by the specified 3D rotation value.

visionOS 1.0+

``` source
nonisolated
func rotation3DEffect(
    _ rotation: Rotation3D,
    anchor: UnitPoint3D = .center
) -> some View
```

## Parameters 

`rotation`  

A rotation to apply to the view’s content.

`anchor`  

The unit point within the view about which to perform the rotation. The default value is center.

## Return Value

A view with rotated content.

## Discussion

This modifier rotates the view’s content without changing the view’s frame. The following code displays a 3D model with a rotation of 45° about the y-axis using the default anchor point at the center of the view:

```
Model3D(named: "robot")
    .rotation3DEffect(Rotation3D(angle: .degrees(45), axis: .y))
```

During an animation, this modifier uses spherical linear interpolation, which produces more natural animations, but doesn’t support rotations over 360 degrees. To specify angles over 360 degrees, consider using `View/rotation3DEffect(_:axis:anchor:)-4enag`.

## See Also

### Scaling, rotating, or transforming a view

func scaledToFill() -> some View

Scales this view to fill its parent.

func scaledToFit() -> some View

Scales this view to fit its parent.

func scaleEffect(_:anchor:)

Scales this view’s rendered output by the given amount in both the horizontal and vertical directions, relative to an anchor point.

func scaleEffect(x: CGFloat, y: CGFloat, anchor: UnitPoint) -> some View

Scales this view’s rendered output by the given horizontal and vertical amounts, relative to an anchor point.

func scaleEffect(x: CGFloat, y: CGFloat, z: CGFloat, anchor: UnitPoint3D) -> some View

Scales this view by the specified horizontal, vertical, and depth factors.

func aspectRatio(_:contentMode:)

Constrains this view’s dimensions to the specified aspect ratio.

func rotationEffect(Angle, anchor: UnitPoint) -> some View

Rotates a view’s rendered output in two dimensions around the specified point.

func rotation3DEffect(Angle, axis: (x: CGFloat, y: CGFloat, z: CGFloat), anchor: UnitPoint, anchorZ: CGFloat, perspective: CGFloat) -> some View

Renders a view’s content as if it’s rotated in three dimensions around the specified axis.

func perspectiveRotationEffect(Angle, axis: (x: CGFloat, y: CGFloat, z: CGFloat), anchor: UnitPoint, anchorZ: CGFloat, perspective: CGFloat) -> some View

Renders a view’s content as if it’s rotated in three dimensions around the specified axis.

func rotation3DEffect(_:axis:anchor:)

Rotates the view’s content by an angle about an axis that you specify as a tuple of elements.

func transformEffect(CGAffineTransform) -> some View

Applies an affine transformation to this view’s rendered output.

func transform3DEffect(AffineTransform3D) -> some View

Applies a 3D transformation to the receiver.

func projectionEffect(ProjectionTransform) -> some View

Applies a projection transformation to this view’s rendered output.

struct ProjectionTransform

enum ContentMode

Constants that define how a view’s content fills the available space.

