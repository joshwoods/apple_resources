

- FamilyControls
- FamilyActivityPicker
-  clipped(antialiased:) 

Instance Method

# clipped(antialiased:)

Clips this view to its bounding rectangular frame.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func clipped(antialiased: Bool = false) -> some View
```

## Parameters 

`antialiased`  

A Boolean value that indicates whether the rendering system applies smoothing to the edges of the clipping rectangle.

## Return Value

A view that clips this view to its bounding frame.

## Discussion

Use the `clipped(antialiased:)` modifier to hide any content that extends beyond the layout bounds of the shape.

By default, a view’s bounding frame is used only for layout, so any content that extends beyond the edges of the frame is still visible.

```
Text("This long text string is clipped")
    .fixedSize()
    .frame(width: 175, height: 100)
    .clipped()
    .border(Color.gray)
```

## See Also

### Masks and Clipping

func mask&lt;Mask>(alignment: Alignment, () -> Mask) -> some View

Masks this view using the alpha channel of the given view.

func clipShape&lt;S>(S, style: FillStyle) -> some View

Sets a clipping shape for this view.

func cornerRadius(CGFloat, antialiased: Bool) -> some View

Clips this view to its bounding frame, with the specified corner radius.

func containerShape&lt;T>(T) -> some View

Sets the container shape to use for any container relative shape within this view.

