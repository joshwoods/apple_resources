

- SwiftUI
- HoverEffectContent
-  clipShape(\_:style:) 

Instance Method

# clipShape(\_:style:)

Sets a clipping shape for the view.

visionOS 2.0+

``` source
func clipShape(
    _ shape: S,
    style: FillStyle = FillStyle()
) -> some HoverEffectContent where S : Shape
```

## Parameters 

`shape`  

The clipping shape to use for the view. The `shape` fills the view’s frame, while maintaining its aspect ratio.

`style`  

The fill style to use when rasterizing `shape`.

## Return Value

An effect that sets the clip shape of a view.

## Discussion

Use `clipShape(_:style:)` to clip the view’s rendered output to the provided shape. By applying a clipping shape, you preserve the parts of the view covered by the shape, while eliminating other parts of the view. The clipping shape itself isn’t visible.

