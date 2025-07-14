

- AppKit
- NSTableViewDataSource
-  tableView(\_:draggingSession:endedAt:operation:) 

Instance Method

# tableView(\_:draggingSession:endedAt:operation:)

Implement this method to determine when a dragging session has ended.

macOS 10.7+

``` source
@MainActor
optional func tableView(
    _ tableView: NSTableView,
    draggingSession session: NSDraggingSession,
    endedAt screenPoint: NSPoint,
    operation: NSDragOperation
)
```

## Parameters 

`tableView`  

The table view.

`session`  

The dragging session.

`screenPoint`  

The ending drag location in screen coordinates.

`operation`  

The drag operation. See NSDragOperation for supported values.

## Discussion

This delegate method can be used to determine when the dragging source operation ended at a specific location, such as the trash, by checking for an operation of delete.

## See Also

### Drag and Drop

Supporting Table View Drag and Drop Through File Promises

Share data between macOS apps during drag and drop by using an item provider.

func tableView(NSTableView, acceptDrop: any NSDraggingInfo, row: Int, dropOperation: NSTableView.DropOperation) -> Bool

Called by `aTableView` when the mouse button is released over a table view that previously decided to allow a drop.

func tableView(NSTableView, namesOfPromisedFilesDroppedAtDestination: URL, forDraggedRowsWith: IndexSet) -> [String]

Returns an array of filenames that represent the `indexSet` rows for a drag to `dropDestination`.

Deprecated

func tableView(NSTableView, validateDrop: any NSDraggingInfo, proposedRow: Int, proposedDropOperation: NSTableView.DropOperation) -> NSDragOperation

Used by `aTableView` to determine a valid drop target.

func tableView(NSTableView, writeRowsWith: IndexSet, to: NSPasteboard) -> Bool

Returns a Boolean value that indicates whether a drag operation is allowed.

Deprecated

func tableView(NSTableView, draggingSession: NSDraggingSession, willBeginAt: NSPoint, forRowIndexes: IndexSet)

Implement this method to determine when a dragging session will begin.

func tableView(NSTableView, updateDraggingItemsForDrag: any NSDraggingInfo)

Implement this method to allow the table to update dragging items as they are dragged over a view.

