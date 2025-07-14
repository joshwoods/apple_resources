

- SwiftUI
-  DropProposal 

Structure

# DropProposal

The behavior of a drop.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15+visionOS 1.0+

``` source
struct DropProposal
```

## Topics

### Creating a drop proposal

init(operation: DropOperation)

let operation: DropOperation

The drop operation that the drop proposes to perform.

## Relationships

### Conforms To

- Sendable

## See Also

### Moving items using item providers

func itemProvider(Optional&lt;() -> NSItemProvider?>) -> some View

Provides a closure that vends the drag representation to be used for a particular data element.

func onDrag&lt;V>(() -> NSItemProvider, preview: () -> V) -> some View

Activates this view as the source of a drag and drop operation.

func onDrag(() -> NSItemProvider) -> some View

Activates this view as the source of a drag and drop operation.

func onDrop(of:isTargeted:perform:)

Defines the destination of a drag-and-drop operation that handles the dropped content with a closure that you specify.

func onDrop(of:delegate:)

Defines the destination of a drag and drop operation using behavior controlled by the delegate that you provide.

protocol DropDelegate

An interface that you implement to interact with a drop operation in a view modified to accept drops.

enum DropOperation

Operation types that determine how a drag and drop session resolves when the user drops a drag item.

struct DropInfo

The current state of a drop.

