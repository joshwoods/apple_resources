

- SwiftUI
- View
-  onDrop(of:isTargeted:perform:) 

Instance Method

# onDrop(of:isTargeted:perform:)

Defines the destination of a drag-and-drop operation that handles the dropped content with a closure that you specify.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
nonisolated
func onDrop(
    of supportedContentTypes: [UTType],
    isTargeted: Binding?,
    perform action: @escaping ([NSItemProvider]) -> Bool
) -> some View
```

Show all declarations

## Parameters 

`supportedContentTypes`  

The uniform type identifiers that describe the types of content this view can accept through drag and drop. If the drag-and-drop operation doesn’t contain any of the supported types, then this drop destination doesn’t activate and `isTargeted` doesn’t update.

`isTargeted`  

A binding that updates when a drag and drop operation enters or exits the drop target area. The binding’s value is `true` when the cursor is inside the area, and `false` when the cursor is outside.

`action`  

A closure that takes the dropped content and responds appropriately. The parameter to `action` contains the dropped items, with types specified by `supportedContentTypes`. Return `true` if the drop operation was successful; otherwise, return `false`.

## Return Value

A view that provides a drop destination for a drag operation of the specified types.

## Discussion

The drop destination is the same size and position as this view.

## See Also

### Moving items using item providers

func itemProvider(Optional&lt;() -> NSItemProvider?>) -> some View

Provides a closure that vends the drag representation to be used for a particular data element.

func onDrag&lt;V>(() -> NSItemProvider, preview: () -> V) -> some View

Activates this view as the source of a drag and drop operation.

func onDrag(() -> NSItemProvider) -> some View

Activates this view as the source of a drag and drop operation.

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

