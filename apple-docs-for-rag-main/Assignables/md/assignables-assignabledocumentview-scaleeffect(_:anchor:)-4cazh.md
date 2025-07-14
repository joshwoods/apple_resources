

- Assignables
- AssignableDocumentView
-  scaleEffect(\_:anchor:) 

Instance Method

# scaleEffect(\_:anchor:)

Scales this view’s rendered output by the given vertical and horizontal size amounts, relative to an anchor point.

AssignablesSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
nonisolated
func scaleEffect(
    _ scale: CGSize,
    anchor: UnitPoint = .center
) -> some View
```

## Parameters 

`scale`  

A CGSize that represents the horizontal and vertical amount to scale the view.

`anchor`  

The point with a default of `UnitPoint/center` that defines the location within the view from which to apply the transformation.

## Discussion

Use `scaleEffect(_:anchor:)` to scale a view by applying a scaling transform of a specific size, specified by `scale`.

```
Image(systemName: "envelope.badge.fill")
    .resizable()
    .frame(width: 100, height: 100, alignment: .center)
    .foregroundColor(Color.red)
    .scaleEffect(CGSize(x: 0.9, y: 1.3), anchor: .leading)
    .border(Color.gray)
```

