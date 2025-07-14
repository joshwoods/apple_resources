

- SwiftUI
-  DropInfo 

Structure

# DropInfo

The current state of a drop.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15+visionOS 1.0+

``` source
struct DropInfo
```

## Topics

### Getting the drop location

var location: CGPoint

The location of the drag in the coordinate space of the drop view.

### Checking for items

func hasItemsConforming(to: [UTType]) -> Bool

Indicates whether at least one item conforms to at least one of the specified uniform type identifiers.

func itemProviders(for: [UTType]) -> [NSItemProvider]

Finds item providers that conform to at least one of the specified uniform type identifiers.

### Deprecated symbols

func hasItemsConforming(to: [String]) -> Bool

Returns whether at least one item conforms to at least one of the specified uniform type identifiers.

Deprecated

func itemProviders(for: [String]) -> [NSItemProvider]

Returns an array of items that each conform to at least one of the specified uniform type identifiers.

Deprecated

### Instance Methods

func hasItemsConforming(to:)

Indicates whether at least one item conforms to at least one of the specified uniform type identifiers.

func itemProviders(for:)

Finds item providers that conform to at least one of the specified uniform type identifiers.

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

struct DropProposal

The behavior of a drop.

enum DropOperation

Operation types that determine how a drag and drop session resolves when the user drops a drag item.

