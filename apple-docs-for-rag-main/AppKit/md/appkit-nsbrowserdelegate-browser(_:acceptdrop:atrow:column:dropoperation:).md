

- AppKit
- NSBrowserDelegate
-  browser(\_:acceptDrop:atRow:column:dropOperation:) 

Instance Method

# browser(\_:acceptDrop:atRow:column:dropOperation:)

Sent to the delegate during a dragging session to determine whether to accept the drop.

macOS 10.5+

``` source
@MainActor
optional func browser(
    _ browser: NSBrowser,
    acceptDrop info: any NSDraggingInfo,
    atRow row: Int,
    column: Int,
    dropOperation: NSBrowser.DropOperation
) -> Bool
```

## Parameters 

`browser`  

The browser.

`info`  

The drag session information.

`row`  

The drop row.

`column`  

The drop column.

`dropOperation`  

The drop location relative to `row`.

## Return Value

true to accept the drop; false to decline it.

## Discussion

This method is required for a browser to be a drag destination. It is invoked after the browser(_:validateDrop:proposedRow:column:dropOperation:) method allows the drop.

The delegate should incorporate the pasteboard data from the dragging session (``` info``.draggingPasteboard ```).

## See Also

### Dragging

func browser(NSBrowser, canDragRowsWith: IndexSet, inColumn: Int, with: NSEvent) -> Bool

Sent to the delegate to determine whether the browser can attempt to initiate a drag of the specified rows for the specified event.

func browser(NSBrowser, draggingImageForRowsWith: IndexSet, inColumn: Int, with: NSEvent, offset: NSPointPointer) -> NSImage?

Sent to the delegate to obtain an image to represent dragged rows during a drag operation on a browser.

func browser(NSBrowser, validateDrop: any NSDraggingInfo, proposedRow: UnsafeMutablePointer&lt;Int>, column: UnsafeMutablePointer&lt;Int>, dropOperation: UnsafeMutablePointer&lt;NSBrowser.DropOperation>) -> NSDragOperation

Sent to the delegate during a dragging session to determine whether a drop should be accepted and to obtain the drop location. This method is required for a browser to be a drag destination.

func browser(NSBrowser, writeRowsWith: IndexSet, inColumn: Int, to: NSPasteboard) -> Bool

Determines whether a drag operation can proceed. This method is required for a browser to be a drag source.

func browser(NSBrowser, namesOfPromisedFilesDroppedAtDestination: URL, forDraggedRowsWith: IndexSet, inColumn: Int) -> [String]

Implements file promise drag operations.

Deprecated

