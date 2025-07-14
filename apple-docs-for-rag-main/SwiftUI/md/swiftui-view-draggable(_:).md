

- SwiftUI
- View
-  draggable(\_:) 

Instance Method

# draggable(\_:)

Activates this view as the source of a drag and drop operation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
nonisolated
func draggable(_ payload: @autoclosure @escaping () -> T) -> some View where T : Transferable
```

## Parameters 

`payload`  

A closure that returns a single instance or a value conforming to Transferable that represents the draggable data from this view.

## Return Value

A view that activates this view as the source of a drag and drop operation, beginning with user gesture input.

## Mentioned in 

Making a view into a drag source

## Discussion

Applying the `draggable(_:)` modifier adds the appropriate gestures for drag and drop to this view. When a drag operation begins, a rendering of this view is generated and used as the preview image.

To customize the default preview, apply a contentShape(_:_:eoFill:) with a dragPreview kind. For example, you can change the preview’s corner radius or use a nested view as the preview.

## See Also

### Moving transferable items

func draggable&lt;V, T>(@autoclosure () -> T, preview: () -> V) -> some View

Activates this view as the source of a drag and drop operation.

func dropDestination&lt;T>(for: T.Type, action: ([T], CGPoint) -> Bool, isTargeted: (Bool) -> Void) -> some View

Defines the destination of a drag and drop operation that handles the dropped content with a closure that you specify.

