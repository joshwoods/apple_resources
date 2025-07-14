

- FamilyControls
- FamilyActivityPicker
-  scaleEffect(\_:anchor:) 

Instance Method

# scaleEffect(\_:anchor:)

Scales this view’s rendered output by the given amount in both the horizontal and vertical directions, relative to an anchor point.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func scaleEffect(
    _ s: CGFloat,
    anchor: UnitPoint = .center
) -> some View
```

## Parameters 

`s`  

The amount to scale the view in the view in both the horizontal and vertical directions.

`anchor`  

The anchor point with a default of `UnitPoint/center` that indicates the starting position for the scale operation.

## Discussion

Use `scaleEffect(_:anchor:)` to apply a horizontally and vertically scaling transform to a view.

```
Image(systemName: "envelope.badge.fill")
    .resizable()
    .frame(width: 100, height: 100, alignment: .center)
    .foregroundColor(Color.red)
    .scaleEffect(2, anchor: .leading)
    .border(Color.gray)
```

