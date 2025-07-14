

- SwiftUI
- View
-  mask(\_:) Deprecated

Instance Method

# mask(\_:)

Masks this view using the alpha channel of the given view.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
nonisolated
func mask(_ mask: Mask) -> some View where Mask : View
```

Deprecated

Use mask(alignment:_:) instead.

## Parameters 

`mask`  

The view whose alpha the rendering system applies to the specified view.

## Discussion

Use `mask(_:)` when you want to apply the alpha (opacity) value of another view to the current view.

This example shows an image masked by rectangle with a 10% opacity:

```
Image(systemName: "envelope.badge.fill")
    .foregroundColor(Color.blue)
    .font(.system(size: 128, weight: .regular))
    .mask(Rectangle().opacity(0.1))
```

## See Also

### Graphics and rendering modifiers

func accentColor(Color?) -> some View

Sets the accent color for this view and the views it contains.

Deprecated

func animation(Animation?) -> some View

Applies the given animation to all animatable values within this view.

Deprecated

func cornerRadius(CGFloat, antialiased: Bool) -> some View

Clips this view to its bounding frame, with the specified corner radius.

Deprecated

