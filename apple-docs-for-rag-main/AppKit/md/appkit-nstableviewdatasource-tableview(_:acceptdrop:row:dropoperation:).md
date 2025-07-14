

- AppKit
- NSTableViewDataSource
-  tableView(\_:acceptDrop:row:dropOperation:) 

Instance Method

# tableView(\_:acceptDrop:row:dropOperation:)

Called by `aTableView` when the mouse button is released over a table view that previously decided to allow a drop.

macOS

``` source
@MainActor
optional func tableView(
    _ tableView: NSTableView,
    acceptDrop info: any NSDraggingInfo,
    row: Int,
    dropOperation: NSTableView.DropOperation
) -> Bool
```

## Parameters 

`tableView`  

The table view that sent the message.

`info`  

An object that contains more information about this dragging operation.

`row`  

The index of the proposed target row.

`dropOperation`  

The type of dragging operation.

## Return Value

true if the drop operation was successful, otherwise false.

## Discussion

The data source should incorporate the data from the dragging pasteboard in the implementation of this method. You can use the draggingPasteboard method to get the data for the drop operation from `info`.

To accept a drop on the second row, `row` would be 2 and `operation` would be `NSTableViewDropOn`. To accept a drop below the last row, `row` would be `[aTableView numberOfRows]` and `operation` would be `NSTableViewDropAbove`.

## See Also

### Drag and Drop

Supporting Table View Drag and Drop Through File Promises

Share data between macOS apps during drag and drop by using an item provider.

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

func tableView(NSTableView, draggingSession: NSDraggingSession, endedAt: NSPoint, operation: NSDragOperation)

Implement this method to determine when a dragging session has ended.

