

- FamilyControls
- FamilyActivityPicker
-  scaleEffect(x:y:anchor:) 

Instance Method

# scaleEffect(x:y:anchor:)

Scales this view’s rendered output by the given horizontal and vertical amounts, relative to an anchor point.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

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

### Scale

func scaledToFill() -> some View

Scales this view to fill its parent.

func scaledToFit() -> some View

Scales this view to fit its parent.

func scaleEffect(CGSize, anchor: UnitPoint) -> some View

Scales this view’s rendered output by the given vertical and horizontal size amounts, relative to an anchor point.

func imageScale(Image.Scale) -> some View

Scales images within the view according to one of the relative sizes available including small, medium, and large images sizes.

func aspectRatio(CGSize, contentMode: ContentMode) -> some View

Constrains this view’s dimensions to the aspect ratio of the given size.

