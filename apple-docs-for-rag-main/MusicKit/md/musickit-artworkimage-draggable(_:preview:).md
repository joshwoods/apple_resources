

- MusicKit
- ArtworkImage
-  draggable(\_:preview:) 

Instance Method

# draggable(\_:preview:)

Activates this view as the source of a drag and drop operation.

MusicKitSwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
nonisolated
func draggable(
    _ payload: @autoclosure @escaping () -> T,
    @ViewBuilder preview: () -> V
) -> some View where V : View, T : Transferable
```

## Parameters 

`payload`  

A closure that returns a single class instance or a value conforming to `Transferable` that represents the draggable data from this view.

`preview`  

A `View` to use as the source for the dragging preview, once the drag operation has begun. The preview is centered over the source view.

## Return Value

A view that activates this view as the source of a drag and drop operation, beginning with user gesture input.

## Discussion

Applying the `draggable(_:preview:)` modifier adds the appropriate gestures for drag and drop to this view. When a drag operation begins, a rendering of `preview` is generated and used as the preview image.

```
var title: String
var body: some View {
    Color.pink
        .frame(width: 400, height: 400)
        .draggable(title) {
             Text("Drop me")
         }
}
```

To customize the lift preview, shown while the system transitions to show your custom `preview`, apply a `View/contentShape(_:_:eoFill:)` with a `ContentShapeKinds/dragPreview` kind. For example, you can change the preview’s corner radius or use a nested view as the preview.

