

- FamilyControls
- FamilyActivityIconView
-  mask(\_:) 

Instance Method

# mask(\_:)

Masks this view using the alpha channel of the given view.

FamilyControlsSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0+visionOSwatchOS 6.0–11.4Deprecated

``` source
nonisolated
func mask(_ mask: Mask) -> some View where Mask : View
```

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

