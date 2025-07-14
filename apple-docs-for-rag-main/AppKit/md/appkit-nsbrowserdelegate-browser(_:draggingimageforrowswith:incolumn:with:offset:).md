

- AppKit
- NSBrowserDelegate
-  browser(\_:draggingImageForRowsWith:inColumn:with:offset:) 

Instance Method

# browser(\_:draggingImageForRowsWith:inColumn:with:offset:)

Sent to the delegate to obtain an image to represent dragged rows during a drag operation on a browser.

macOS 10.5+

``` source
@MainActor
optional func browser(
    _ browser: NSBrowser,
    draggingImageForRowsWith rowIndexes: IndexSet,
    inColumn column: Int,
    with event: NSEvent,
    offset dragImageOffset: NSPointPointer
) -> NSImage?
```

## Parameters 

`browser`  

The browser.

`rowIndexes`  

The indexes of the rows the user is dragging.

`column`  

The column containing the rows the user is dragging.

`event`  

The drag event.

`dragImageOffset`  

The offset for the returned image:

- NSZeroPoint: Centers the image under the pointer.

## Return Value

An image representing the visible rows identified by `rowIndexes`.

## See Also

### Related Documentation

func draggingImageForRows(with: IndexSet, inColumn: Int, with: NSEvent, offset: NSPointPointer?) -> NSImage?

Provides an image to represent dragged rows during a drag operation on the browser.

### Dragging

func browser(NSBrowser, canDragRowsWith: IndexSet, inColumn: Int, with: NSEvent) -> Bool

Sent to the delegate to determine whether the browser can attempt to initiate a drag of the specified rows for the specified event.

func browser(NSBrowser, validateDrop: any NSDraggingInfo, proposedRow: UnsafeMutablePointer&lt;Int>, column: UnsafeMutablePointer&lt;Int>, dropOperation: UnsafeMutablePointer&lt;NSBrowser.DropOperation>) -> NSDragOperation

Sent to the delegate during a dragging session to determine whether a drop should be accepted and to obtain the drop location. This method is required for a browser to be a drag destination.

func browser(NSBrowser, acceptDrop: any NSDraggingInfo, atRow: Int, column: Int, dropOperation: NSBrowser.DropOperation) -> Bool

Sent to the delegate during a dragging session to determine whether to accept the drop.

func browser(NSBrowser, writeRowsWith: IndexSet, inColumn: Int, to: NSPasteboard) -> Bool

Determines whether a drag operation can proceed. This method is required for a browser to be a drag source.

func browser(NSBrowser, namesOfPromisedFilesDroppedAtDestination: URL, forDraggedRowsWith: IndexSet, inColumn: Int) -> [String]

Implements file promise drag operations.

Deprecated

