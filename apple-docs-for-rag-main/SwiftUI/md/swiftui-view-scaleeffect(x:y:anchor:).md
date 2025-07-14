

- SwiftUI
- View
-  scaleEffect(x:y:anchor:) 

Instance Method

# scaleEffect(x:y:anchor:)

Scales this view’s rendered output by the given horizontal and vertical amounts, relative to an anchor point.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func scaleEffect(
    x: CGFloat = 1.0,
    y: CGFloat = 1.0,
    anchor: UnitPoint = .center
) -> some View
```

## Parameters 

`x`  

An amount that represents the horizontal amount to scale the view. The default value is `1.0`.

`y`  

An amount that represents the vertical amount to scale the view. The default value is `1.0`.

`anchor`  

The anchor point that indicates the starting position for the scale operation.

## Discussion

Use `scaleEffect(x:y:anchor:)` to apply a scaling transform to a view by a specific horizontal and vertical amount.

```
Image(systemName: "envelope.badge.fill")
    .resizable()
    .frame(width: 100, height: 100, alignment: .center)
    .foregroundColor(Color.red)
    .scaleEffect(x: 0.5, y: 0.5, anchor: .bottomTrailing)
    .border(Color.gray)
```

## See Also

### Scaling, rotating, or transforming a view

func scaledToFill() -> some View

Scales this view to fill its parent.

func scaledToFit() -> some View

Scales this view to fit its parent.

func scaleEffect(_:anchor:)

Scales this view’s rendered output by the given amount in both the horizontal and vertical directions, relative to an anchor point.

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

func rotation3DEffect(Rotation3D, anchor: UnitPoint3D) -> some View

Rotates the view’s content by the specified 3D rotation value.

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

