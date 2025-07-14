

- RealityKit
- RealityViewAttachmentBuilderContent
-  onDrag(\_:preview:) 

Instance Method

# onDrag(\_:preview:)

Activates this view as the source of a drag and drop operation.

RealityKitSwiftUIiOS 15.0+iPadOS 15.0+macOS 12.0+visionOS

``` source
nonisolated
func onDrag(
    _ data: @escaping () -> NSItemProvider,
    @ViewBuilder preview: () -> V
) -> some View where V : View
```

## Parameters 

`data`  

A closure that returns a single NSItemProvider that represents the draggable data from this view.

`preview`  

A `View` to use as the source for the dragging preview, once the drag operation has begun. The preview is centered over the source view.

## Return Value

A view that activates this view as the source of a drag-and- drop operation, beginning with user gesture input.

## Discussion

Applying the `onDrag(_:preview:)` modifier adds the appropriate gestures for drag and drop to this view. When a drag operation begins, a rendering of `preview` is generated and used as the preview image.

To customize the lift preview, shown while the system transitions to show your custom `preview`, apply a `View/contentShape(_:_:eoFill:)` with a `ContentShapeKinds/dragPreview` kind. For example, you can change the preview’s corner radius or use a nested view as the preview.

