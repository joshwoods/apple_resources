

- FamilyControls
- FamilyActivityPicker
-  scaledToFit() 

Instance Method

# scaledToFit()

Scales this view to fit its parent.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func scaledToFit() -> some View
```

## Return Value

A view that scales this view to fit its parent, maintaining this view’s aspect ratio.

## Discussion

Use `scaledToFit()` to scale this view to fit its parent, while maintaining the view’s aspect ratio as the view scales.

```
Circle()
    .fill(Color.pink)
    .scaledToFit()
    .frame(width: 300, height: 150)
    .border(Color(white: 0.75))
```

This method is equivalent to calling `View/aspectRatio(_:contentMode:)` with a `nil` aspectRatio and a content mode of `ContentMode/fit`.

## See Also

### Scale

func scaledToFill() -> some View

Scales this view to fill its parent.

func scaleEffect(CGSize, anchor: UnitPoint) -> some View

Scales this view’s rendered output by the given vertical and horizontal size amounts, relative to an anchor point.

func scaleEffect(x: CGFloat, y: CGFloat, anchor: UnitPoint) -> some View

Scales this view’s rendered output by the given horizontal and vertical amounts, relative to an anchor point.

func imageScale(Image.Scale) -> some View

Scales images within the view according to one of the relative sizes available including small, medium, and large images sizes.

func aspectRatio(CGSize, contentMode: ContentMode) -> some View

Constrains this view’s dimensions to the aspect ratio of the given size.

