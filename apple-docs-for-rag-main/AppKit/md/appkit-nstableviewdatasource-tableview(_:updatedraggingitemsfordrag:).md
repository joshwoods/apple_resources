

- AppKit
- NSTableViewDataSource
-  tableView(\_:updateDraggingItemsForDrag:) 

Instance Method

# tableView(\_:updateDraggingItemsForDrag:)

Implement this method to allow the table to update dragging items as they are dragged over a view.

macOS 10.7+

``` source
@MainActor
optional func tableView(
    _ tableView: NSTableView,
    updateDraggingItemsForDrag draggingInfo: any NSDraggingInfo
)
```

## Parameters 

`tableView`  

The table view.

`draggingInfo`  

The dragging information.

## Discussion

Required for multi-image dragging. Typically this will involve invoking enumerateDraggingItems(options:for:classes:searchOptions:using:) on the `draggingInfo` parameter value and setting the `draggingItem` object’s imageComponentsProvider to a proper image based on the content.

For view-based table views, you can use the `NSTableCellView` method draggingImageComponents. For cell-based tables, use the `NSCell` method draggingImageComponents(withFrame:in:).

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

func tableView(NSTableView, draggingSession: NSDraggingSession, endedAt: NSPoint, operation: NSDragOperation)

Implement this method to determine when a dragging session has ended.

