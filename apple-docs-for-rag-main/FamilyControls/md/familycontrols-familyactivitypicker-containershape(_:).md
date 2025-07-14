

- FamilyControls
- FamilyActivityPicker
-  containerShape(\_:) 

Instance Method

# containerShape(\_:)

Sets the container shape to use for any container relative shape within this view.

FamilyControlsSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+watchOS 8.0+

``` source
nonisolated
func containerShape(_ shape: T) -> some View where T : InsettableShape
```

## Discussion

The example below defines a view that shows its content with a rounded rectangle background and the same container shape. Any `ContainerRelativeShape` within the `content` matches the rounded rectangle shape from this container inset as appropriate.

```
struct PlatterContainer : View {
    @ViewBuilder var content: Content
    var body: some View {
        content
            .padding()
            .containerShape(shape)
            .background(shape.fill(.background))
    }
    var shape: RoundedRectangle { RoundedRectangle(cornerRadius: 20) }
}
```

## See Also

### Masks and Clipping

func mask&lt;Mask>(alignment: Alignment, () -> Mask) -> some View

Masks this view using the alpha channel of the given view.

func clipped(antialiased: Bool) -> some View

Clips this view to its bounding rectangular frame.

func clipShape&lt;S>(S, style: FillStyle) -> some View

Sets a clipping shape for this view.

func cornerRadius(CGFloat, antialiased: Bool) -> some View

Clips this view to its bounding frame, with the specified corner radius.

