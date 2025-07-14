

- AppKit
- NSDraggingInfo
-  draggingSourceOperationMask 

Instance Property

# draggingSourceOperationMask

Information about the dragging operation and the data it contains.

macOS

``` source
@MainActor
var draggingSourceOperationMask: NSDragOperation { get }
```

**Required**

## Discussion

The dragging source (NSDraggingSource) declares the dragging operation mask through draggingSession(_:sourceOperationMaskFor:).

If the source doesn’t permit dragging operations, the value of the dragging source operation mask is NSDragOperationNone, or the empty option set in Swift (`[]`). If the source permits dragging operations, the value of the dragging source operation mask is the result of a bitwise OR operation on one or more of the NSDragOperation constants in Objective-C, or an option set containing one or more of the NSDragOperation constants in Swift.

If the user holds down a modifier key during the dragging session and the dragging source allows modifier keys to affect the drag operation, the system combines the dragging source operation mask with the value that corresponds to the modifier key. You control whether the modifier keys can affect the drag operation using the dragging source’s ignoreModifierKeys(for:) method.

| Modifier Key | Dragging Operation |
|----|----|
| Option | copy |
| Command | move |
| Option and Command | link |

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

var draggingLocation: NSPoint

The current location of the mouse pointer in the base coordinate system of the destination object’s window.

**Required**

var draggingDestinationWindow: NSWindow?

The destination window for the dragging operation.

**Required**

var numberOfValidItemsForDrop: Int

The number of valid items for a drop operation.

**Required**

func namesOfPromisedFilesDropped(atDestination: URL) -> [String]?

Sets the drop location for promised files and returns the names of the files that the receiver promises to create there.

**Required**

Deprecated

