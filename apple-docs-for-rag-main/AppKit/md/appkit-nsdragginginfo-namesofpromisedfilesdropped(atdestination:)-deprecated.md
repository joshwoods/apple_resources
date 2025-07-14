

- AppKit
- NSDraggingInfo
-  namesOfPromisedFilesDropped(atDestination:) Deprecated

Instance Method

# namesOfPromisedFilesDropped(atDestination:)

Sets the drop location for promised files and returns the names of the files that the receiver promises to create there.

macOS 10.0–10.13Deprecated

``` source
func namesOfPromisedFilesDropped(atDestination dropDestination: URL) -> [String]?
```

**Required**

Deprecated

Use NSFilePromiseReceiver objects instead

## Parameters 

`dropDestination`  

A URL object specifying the drop location for promised files.

## Return Value

An array of file names, which are not full paths.

## Discussion

Drag destinations should invoke this method within their performDragOperation: method. The source may or may not have created the files by the time this method returns.

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

var numberOfValidItemsForDrop: Int

The number of valid items for a drop operation.

**Required**

