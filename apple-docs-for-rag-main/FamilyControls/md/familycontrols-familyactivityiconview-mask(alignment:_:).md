

- FamilyControls
- FamilyActivityIconView
-  mask(alignment:\_:) 

Instance Method

# mask(alignment:\_:)

Masks this view using the alpha channel of the given view.

FamilyControlsSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+watchOS 8.0+

``` source
nonisolated
func mask(
    alignment: Alignment = .center,
    @ViewBuilder _ mask: () -> Mask
) -> some View where Mask : View
```

## Parameters 

`alignment`  

The alignment for `mask` in relation to this view.

`mask`  

The view whose alpha the rendering system applies to the specified view.

## Discussion

Use `mask(_:)` when you want to apply the alpha (opacity) value of another view to the current view.

This example shows an image masked by rectangle with a 10% opacity:

```
Image(systemName: "envelope.badge.fill")
    .foregroundColor(Color.blue)
    .font(.system(size: 128, weight: .regular))
    .mask {
        Rectangle().opacity(0.1)
    }
```

