

- AppKit
- NSDraggingInfo
-  numberOfValidItemsForDrop 

Instance Property

# numberOfValidItemsForDrop

The number of valid items for a drop operation.

macOS 10.7+

``` source
@MainActor
var numberOfValidItemsForDrop: Int { get set }
```

**Required**

## Discussion

During draggingEntered: or draggingUpdated:, you are responsible for returning the drag operation. In some cases, you may accept some, but not all items on the dragging pasteboard. (For example, your application may only accept image files.)

If you only accept some of the items, set this property to the number of items accepted so the drag manager can update the drag count badge.

When updateDraggingItemsForDrag(_:) is called, you should set the image of non-valid dragging items to `nil`. If none of the drag items are valid then you should not `updateItems:`, simply return NSDragOperationNone from your implementation of draggingEntered: and, or draggingUpdated: and do not modify any drag item properties.

## See Also

### Obtaining information about the dragging session

var draggingPasteboard: NSPasteboard

The pasteboard object that holds the dragged data.

**Required**

var draggingSequenceNumber: Int

A number that uniquely identifies the dragging session.

**Required**

var draggingSource: Any?

The source, or owner, of the dragged data.

**Required**

var draggingSourceOperationMask: NSDragOperation

Information about the dragging operation and the data it contains.

**Required**

var draggingLocation: NSPoint

The current location of the mouse pointer in the base coordinate system of the destination object’s window.

**Required**

var draggingDestinationWindow: NSWindow?

The destination window for the dragging operation.

**Required**

func namesOfPromisedFilesDropped(atDestination: URL) -> [String]?

Sets the drop location for promised files and returns the names of the files that the receiver promises to create there.

**Required**

Deprecated

