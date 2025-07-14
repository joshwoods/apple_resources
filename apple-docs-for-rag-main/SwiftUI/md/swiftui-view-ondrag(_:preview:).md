

- SwiftUI
- View
-  onDrag(\_:preview:) 

Instance Method

# onDrag(\_:preview:)

Activates this view as the source of a drag and drop operation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

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

A View to use as the source for the dragging preview, once the drag operation has begun. The preview is centered over the source view.

## Return Value

A view that activates this view as the source of a drag-and- drop operation, beginning with user gesture input.

## Discussion

Applying the `onDrag(_:preview:)` modifier adds the appropriate gestures for drag and drop to this view. When a drag operation begins, a rendering of `preview` is generated and used as the preview image.

To customize the lift preview, shown while the system transitions to show your custom `preview`, apply a contentShape(_:_:eoFill:) with a dragPreview kind. For example, you can change the preview’s corner radius or use a nested view as the preview.

## See Also

### Moving items using item providers

func itemProvider(Optional&lt;() -> NSItemProvider?>) -> some View

Provides a closure that vends the drag representation to be used for a particular data element.

func onDrag(() -> NSItemProvider) -> some View

Activates this view as the source of a drag and drop operation.

func onDrop(of:isTargeted:perform:)

Defines the destination of a drag-and-drop operation that handles the dropped content with a closure that you specify.

func onDrop(of:delegate:)

Defines the destination of a drag and drop operation using behavior controlled by the delegate that you provide.

protocol DropDelegate

An interface that you implement to interact with a drop operation in a view modified to accept drops.

struct DropProposal

The behavior of a drop.

enum DropOperation

Operation types that determine how a drag and drop session resolves when the user drops a drag item.

struct DropInfo

The current state of a drop.

