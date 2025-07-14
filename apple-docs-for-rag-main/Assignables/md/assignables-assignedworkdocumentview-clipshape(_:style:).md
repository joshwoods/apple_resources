

- Assignables
- AssignedWorkDocumentView
-  clipShape(\_:style:) 

Instance Method

# clipShape(\_:style:)

Sets a clipping shape for this view.

AssignablesSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
nonisolated
func clipShape(
    _ shape: S,
    style: FillStyle = FillStyle()
) -> some View where S : Shape
```

## Parameters 

`shape`  

The clipping shape to use for this view. The `shape` fills the view’s frame, while maintaining its aspect ratio.

`style`  

The fill style to use when rasterizing `shape`.

## Return Value

A view that clips this view to `shape`, using `style` to define the shape’s rasterization.

## Discussion

Use `clipShape(_:style:)` to clip the view to the provided shape. By applying a clipping shape to a view, you preserve the parts of the view covered by the shape, while eliminating other parts of the view. The clipping shape itself isn’t visible.

For example, this code applies a circular clipping shape to a `Text` view:

```
Text("Clipped text in a circle")
    .frame(width: 175, height: 100)
    .foregroundColor(Color.white)
    .background(Color.black)
    .clipShape(Circle())
```

The resulting view shows only the portion of the text that lies within the bounds of the circle.

