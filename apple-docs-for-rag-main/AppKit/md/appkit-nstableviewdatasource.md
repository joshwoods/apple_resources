

- AppKit
-  NSTableViewDataSource 

Protocol

# NSTableViewDataSource

A set of methods that a table view uses to provide data to a table view and to allow the editing of the table view’s data source object.

macOS

``` source
protocol NSTableViewDataSource : NSObjectProtocol
```

## Overview

Some of the methods in this protocol, such as tableView(_:objectValueFor:row:) and numberOfRows(in:) along with other methods that return data, are called frequently, so they must be efficient.

Note

View-based table views must not use the tableView(_:setObjectValue:for:row:) method for setting values. Instead the views must explicitly set the values for the fields, or use Cocoa bindings. Likewise, use target/action for editing. See Table View Programming Guide for Mac for more information on populating view-based and cell-based table views.

If you’re not using Cocoa bindings to provide data to the table view, the following methods are required:

- numberOfRows(in:)

- tableView(_:objectValueFor:row:)

- tableView(_:setObjectValue:for:row:) (cell-based tables only)

To learn more about Cocoa bindings, see Cocoa Bindings Programming Topics.

## Topics

### Getting Values

func numberOfRows(in: NSTableView) -> Int

Returns the number of records managed for `aTableView` by the data source object.

func tableView(NSTableView, objectValueFor: NSTableColumn?, row: Int) -> Any?

Called by the table view to return the data object associated with the specified row and column.

### Setting Values

func tableView(NSTableView, setObjectValue: Any?, for: NSTableColumn?, row: Int)

Sets the data object for an item in the specified row and column.

### Implementing Pasteboard Support

func tableView(NSTableView, pasteboardWriterForRow: Int) -> (any NSPasteboardWriting)?

Called to allow the table to support multiple item dragging.

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

func tableView(NSTableView, draggingSession: NSDraggingSession, endedAt: NSPoint, operation: NSDragOperation)

Implement this method to determine when a dragging session has ended.

### Sorting

func tableView(NSTableView, sortDescriptorsDidChange: [NSSortDescriptor])

Called by `aTableView` to indicate that sorting may need to be done.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSTableViewDiffableDataSource
- NSTableViewDiffableDataSourceReference

## See Also

### Management

protocol NSTableViewDelegate

A set of optional methods you implement in a table view delegate to customize the behavior of the table view.

class NSTableViewDiffableDataSource

The object you use to manage data and provide items for a table view.

