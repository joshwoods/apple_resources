

- AppKit
- NSTableViewDataSource
-  tableView(\_:namesOfPromisedFilesDroppedAtDestination:forDraggedRowsWith:) Deprecated

Instance Method

# tableView(\_:namesOfPromisedFilesDroppedAtDestination:forDraggedRowsWith:)

Returns an array of filenames that represent the `indexSet` rows for a drag to `dropDestination`.

macOS 10.0–10.13Deprecated

``` source
optional func tableView(
    _ tableView: NSTableView,
    namesOfPromisedFilesDroppedAtDestination dropDestination: URL,
    forDraggedRowsWith indexSet: IndexSet
) -> [String]
```

Deprecated

Use NSFilePromiseReceiver objects instead

## Parameters 

`tableView`  

The table view that sent the message.

`dropDestination`  

The drop location where the files are created.

`indexSet`  

The indexes of the items being dragged.

## Return Value

An array of filenames (not full paths) for the created files that the receiver promises to create.

## Discussion

This method is called when a destination has accepted a promise drag.

For more information on file promise dragging, see documentation on the NSDraggingSource protocol and namesOfPromisedFilesDropped(atDestination:).

## See Also

### Drag and Drop

Supporting Table View Drag and Drop Through File Promises

Share data between macOS apps during drag and drop by using an item provider.

func tableView(NSTableView, acceptDrop: any NSDraggingInfo, row: Int, dropOperation: NSTableView.DropOperation) -> Bool

Called by `aTableView` when the mouse button is released over a table view that previously decided to allow a drop.

func tableView(NSTableView, validateDrop: any NSDraggingInfo, proposedRow: Int, proposedDropOperation: NSTableView.DropOperation) -> NSDragOperation

Used by `aTableView` to determine a valid drop target.

func tableView(NSTableView, writeRowsWith: IndexSet, to: NSPasteboard) -> Bool

Returns a Boolean value that indicates whether a drag operation is allowed.

Deprecated

func tableView(NSTableView, draggingSession: NSDraggingSession, willBeginAt: NSPoint, forRowIndexes: IndexSet)

Implement this method to determine when a dragging session will begin.

func tableView(NSTableView, updateDraggingItemsForDrag: any NSDraggingInfo)

Implement this method to allow the table to update dragging items as they are dragged over a view.

func tableView(NSTableView, draggingSession: NSDraggingSession, endedAt: NSPoint, operation: NSDragOperation)

Implement this method to determine when a dragging session has ended.

