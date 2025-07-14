

- AppKit
- NSTableViewDataSource
-  tableView(\_:draggingSession:willBeginAt:forRowIndexes:) 

Instance Method

# tableView(\_:draggingSession:willBeginAt:forRowIndexes:)

Implement this method to determine when a dragging session will begin.

macOS 10.7+

``` source
@MainActor
optional func tableView(
    _ tableView: NSTableView,
    draggingSession session: NSDraggingSession,
    willBeginAt screenPoint: NSPoint,
    forRowIndexes rowIndexes: IndexSet
)
```

## Parameters 

`tableView`  

The table view.

`session`  

The dragging session.

`screenPoint`  

The initial drag location in screen coordinates.

`rowIndexes`  

The indexes of the rows to be dragged, excluding rows that were not dragged due to tableView(_:pasteboardWriterForRow:) returning `nil`.

## Discussion

Implement this method to know when the dragging session is about to begin and to potentially modify the dragging session.

The dragged item order will directly match the pasteboard writer array used to begin the dragging session with the `NSView` method beginDraggingSession(with:event:source:). Hence, the order is deterministic, and can be used in tableView(_:acceptDrop:row:dropOperation:) when enumerating the NSDraggingInfo pasteboard classes.

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

func tableView(NSTableView, updateDraggingItemsForDrag: any NSDraggingInfo)

Implement this method to allow the table to update dragging items as they are dragged over a view.

func tableView(NSTableView, draggingSession: NSDraggingSession, endedAt: NSPoint, operation: NSDragOperation)

Implement this method to determine when a dragging session has ended.

