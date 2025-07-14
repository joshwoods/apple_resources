

- AppKit
- NSDraggingInfo
-  draggingPasteboard 

Instance Property

# draggingPasteboard

The pasteboard object that holds the dragged data.

macOS

``` source
@MainActor
var draggingPasteboard: NSPasteboard { get }
```

**Required**

## Discussion

The dragging operation that is ultimately performed utilizes this pasteboard data and not the image returned by the draggedImage method.

## See Also

### Related Documentation

Drag and Drop Programming Topics

### Obtaining information about the dragging session

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

var numberOfValidItemsForDrop: Int

The number of valid items for a drop operation.

**Required**

func namesOfPromisedFilesDropped(atDestination: URL) -> [String]?

Sets the drop location for promised files and returns the names of the files that the receiver promises to create there.

**Required**

Deprecated

