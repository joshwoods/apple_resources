

- RealityKit
- ObjectCapturePointCloudView
-  draggable(\_:) 

Instance Method

# draggable(\_:)

Activates this view as the source of a drag and drop operation.

RealityKitSwiftUIiOS 16.0+iPadOS 16.0+macOS 13.0+

``` source
nonisolated
func draggable(_ payload: @autoclosure @escaping () -> T) -> some View where T : Transferable
```

## Parameters 

`payload`  

A closure that returns a single instance or a value conforming to Transferable that represents the draggable data from this view.

## Return Value

A view that activates this view as the source of a drag and drop operation, beginning with user gesture input.

## Discussion

Applying the `draggable(_:)` modifier adds the appropriate gestures for drag and drop to this view. When a drag operation begins, a rendering of this view is generated and used as the preview image.

To customize the default preview, apply a `View/contentShape(_:_:eoFill:)` with a `ContentShapeKinds/dragPreview` kind. For example, you can change the preview’s corner radius or use a nested view as the preview.

