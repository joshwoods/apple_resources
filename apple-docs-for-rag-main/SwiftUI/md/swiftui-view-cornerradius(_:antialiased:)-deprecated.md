

- SwiftUI
- View
-  cornerRadius(\_:antialiased:) Deprecated

Instance Method

# cornerRadius(\_:antialiased:)

Clips this view to its bounding frame, with the specified corner radius.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
nonisolated
func cornerRadius(
    _ radius: CGFloat,
    antialiased: Bool = true
) -> some View
```

Deprecated

Use clipShape(_:style:) or fill(style:) instead.

## Parameters 

`antialiased`  

A Boolean value that indicates whether the rendering system applies smoothing to the edges of the clipping rectangle.

## Return Value

A view that clips this view to its bounding frame with the specified corner radius.

## Discussion

By default, a view’s bounding frame only affects its layout, so any content that extends beyond the edges of the frame remains visible. Use `cornerRadius(_:antialiased:)` to hide any content that extends beyond these edges while applying a corner radius.

The following code applies a corner radius of 25 to a text view:

```
Text("Rounded Corners")
    .frame(width: 175, height: 75)
    .foregroundColor(Color.white)
    .background(Color.black)
    .cornerRadius(25)
```

## See Also

### Graphics and rendering modifiers

func accentColor(Color?) -> some View

Sets the accent color for this view and the views it contains.

Deprecated

func mask&lt;Mask>(Mask) -> some View

Masks this view using the alpha channel of the given view.

Deprecated

func animation(Animation?) -> some View

Applies the given animation to all animatable values within this view.

Deprecated

