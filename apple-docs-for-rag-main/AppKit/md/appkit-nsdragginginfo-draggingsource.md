

- AppKit
- NSDraggingInfo
-  draggingSource 

Instance Property

# draggingSource

The source, or owner, of the dragged data.

macOS

``` source
@MainActor
var draggingSource: Any? { get }
```

**Required**

## Discussion

This method returns `nil` if the source is not in the same application as the destination. The dragging source implements methods from the NSDraggingSource protocol.

## See Also

### Obtaining information about the dragging session

var draggingPasteboard: NSPasteboard

The pasteboard object that holds the dragged data.

**Required**

var draggingSequenceNumber: Int

A number that uniquely identifies the dragging session.

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

var numberOfValidItemsForDrop: Int

The number of valid items for a drop operation.

**Required**

func namesOfPromisedFilesDropped(atDestination: URL) -> [String]?

Sets the drop location for promised files and returns the names of the files that the receiver promises to create there.

**Required**

Deprecated

