

- AppKit
- NSBrowserDelegate
-  browser(\_:canDragRowsWith:inColumn:with:) 

Instance Method

# browser(\_:canDragRowsWith:inColumn:with:)

Sent to the delegate to determine whether the browser can attempt to initiate a drag of the specified rows for the specified event.

macOS 10.5+

``` source
@MainActor
optional func browser(
    _ browser: NSBrowser,
    canDragRowsWith rowIndexes: IndexSet,
    inColumn column: Int,
    with event: NSEvent
) -> Bool
```

## Parameters 

`browser`  

The browser.

`rowIndexes`  

The rows the user is dragging.

`column`  

The column containing the rows the user is dragging.

`event`  

The drag event.

## Return Value

true to allow the drag operation; false to disallow it.

## See Also

### Related Documentation

func canDragRows(with: IndexSet, inColumn: Int, with: NSEvent) -> Bool

Indicates whether the browser can attempt to initiate a drag of the given rows for the given event.

### Dragging

func browser(NSBrowser, draggingImageForRowsWith: IndexSet, inColumn: Int, with: NSEvent, offset: NSPointPointer) -> NSImage?

Sent to the delegate to obtain an image to represent dragged rows during a drag operation on a browser.

func browser(NSBrowser, validateDrop: any NSDraggingInfo, proposedRow: UnsafeMutablePointer&lt;Int>, column: UnsafeMutablePointer&lt;Int>, dropOperation: UnsafeMutablePointer&lt;NSBrowser.DropOperation>) -> NSDragOperation

Sent to the delegate during a dragging session to determine whether a drop should be accepted and to obtain the drop location. This method is required for a browser to be a drag destination.

func browser(NSBrowser, acceptDrop: any NSDraggingInfo, atRow: Int, column: Int, dropOperation: NSBrowser.DropOperation) -> Bool

Sent to the delegate during a dragging session to determine whether to accept the drop.

func browser(NSBrowser, writeRowsWith: IndexSet, inColumn: Int, to: NSPasteboard) -> Bool

Determines whether a drag operation can proceed. This method is required for a browser to be a drag source.

func browser(NSBrowser, namesOfPromisedFilesDroppedAtDestination: URL, forDraggedRowsWith: IndexSet, inColumn: Int) -> [String]

Implements file promise drag operations.

Deprecated

