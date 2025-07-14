

- AppKit
- NSBrowserDelegate
-  browser(\_:writeRowsWith:inColumn:to:) 

Instance Method

# browser(\_:writeRowsWith:inColumn:to:)

Determines whether a drag operation can proceed. This method is required for a browser to be a drag source.

macOS 10.5+

``` source
@MainActor
optional func browser(
    _ browser: NSBrowser,
    writeRowsWith rowIndexes: IndexSet,
    inColumn column: Int,
    to pasteboard: NSPasteboard
) -> Bool
```

## Parameters 

`browser`  

The browser.

`rowIndexes`  

The indexes of the rows the user is dragging.

`column`  

The index of the column containing the dragged rows.

`pasteboard`  

The pasteboard containing the content from the dragged rows.

## Return Value

true to allow the dragging operation to proceed (see discussion for further details); false to disallow it.

## Discussion

This method is called after a drag operation has been allowed to start (browser(_:canDragRowsWith:inColumn:with:) returns true), but before it actually begins.

## See Also

### Dragging

func browser(NSBrowser, canDragRowsWith: IndexSet, inColumn: Int, with: NSEvent) -> Bool

Sent to the delegate to determine whether the browser can attempt to initiate a drag of the specified rows for the specified event.

func browser(NSBrowser, draggingImageForRowsWith: IndexSet, inColumn: Int, with: NSEvent, offset: NSPointPointer) -> NSImage?

Sent to the delegate to obtain an image to represent dragged rows during a drag operation on a browser.

func browser(NSBrowser, validateDrop: any NSDraggingInfo, proposedRow: UnsafeMutablePointer&lt;Int>, column: UnsafeMutablePointer&lt;Int>, dropOperation: UnsafeMutablePointer&lt;NSBrowser.DropOperation>) -> NSDragOperation

Sent to the delegate during a dragging session to determine whether a drop should be accepted and to obtain the drop location. This method is required for a browser to be a drag destination.

func browser(NSBrowser, acceptDrop: any NSDraggingInfo, atRow: Int, column: Int, dropOperation: NSBrowser.DropOperation) -> Bool

Sent to the delegate during a dragging session to determine whether to accept the drop.

func browser(NSBrowser, namesOfPromisedFilesDroppedAtDestination: URL, forDraggedRowsWith: IndexSet, inColumn: Int) -> [String]

Implements file promise drag operations.

Deprecated

