

- AppKit
- NSTableViewDataSource
-  tableView(\_:writeRowsWith:to:) Deprecated

Instance Method

# tableView(\_:writeRowsWith:to:)

Returns a Boolean value that indicates whether a drag operation is allowed.

macOS 10.4–10.15Deprecated

``` source
optional func tableView(
    _ tableView: NSTableView,
    writeRowsWith rowIndexes: IndexSet,
    to pboard: NSPasteboard
) -> Bool
```

Deprecated

Use -tableView:pasteboardWriterForRow: instead

## Parameters 

`tableView`  

The table view that sent the message.

`rowIndexes`  

An index set of row numbers that will be participating in the drag.

`pboard`  

The pasteboard to which to write the drag data.

## Return Value

`YES` if the drag operation is allowed, `NO` otherwise.

## Discussion

Called by `aTableView` after it has been determined that a drag should begin, but before the drag has been started.

To refuse the drag, return false. To start a drag, return true and place the drag data onto `pboard` (data, owner, and so on). The drag image and other drag-related information will be set up and provided by the table view once this call returns with true.

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

func tableView(NSTableView, draggingSession: NSDraggingSession, willBeginAt: NSPoint, forRowIndexes: IndexSet)

Implement this method to determine when a dragging session will begin.

func tableView(NSTableView, updateDraggingItemsForDrag: any NSDraggingInfo)

Implement this method to allow the table to update dragging items as they are dragged over a view.

func tableView(NSTableView, draggingSession: NSDraggingSession, endedAt: NSPoint, operation: NSDragOperation)

Implement this method to determine when a dragging session has ended.

