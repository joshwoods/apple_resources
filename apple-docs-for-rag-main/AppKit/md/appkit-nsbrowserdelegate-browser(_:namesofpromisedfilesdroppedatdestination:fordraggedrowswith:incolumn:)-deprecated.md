

- AppKit
- NSBrowserDelegate
-  browser(\_:namesOfPromisedFilesDroppedAtDestination:forDraggedRowsWith:inColumn:) Deprecated

Instance Method

# browser(\_:namesOfPromisedFilesDroppedAtDestination:forDraggedRowsWith:inColumn:)

Implements file promise drag operations.

macOS 10.5–10.13Deprecated

``` source
optional func browser(
    _ browser: NSBrowser,
    namesOfPromisedFilesDroppedAtDestination dropDestination: URL,
    forDraggedRowsWith rowIndexes: IndexSet,
    inColumn column: Int
) -> [String]
```

Deprecated

Use NSFilePromiseReceiver objects instead

## Parameters 

`browser`  

The browser.

`dropDestination`  

The drop filesystem location.

`rowIndexes`  

The indexes of the rows the user is dropping.

`column`  

The index of the column containing the rows the user is dropping.

## Return Value

Filenames (not pathnames) for the actual files represented by the rows the user is dropping.

## Discussion

Note that file promise drag operation support requires adding the data type filePromise to the pasteboard in the browser(_:writeRowsWith:inColumn:to:) method.

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

func browser(NSBrowser, writeRowsWith: IndexSet, inColumn: Int, to: NSPasteboard) -> Bool

Determines whether a drag operation can proceed. This method is required for a browser to be a drag source.

