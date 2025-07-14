

- AppKit
-  NSTableViewDelegate 

Protocol

# NSTableViewDelegate

A set of optional methods you implement in a table view delegate to customize the behavior of the table view.

macOS

``` source
protocol NSTableViewDelegate : NSControlTextEditingDelegate
```

## Overview

Using a table view delegate allows you to customize a table view’s behavior without creating a table view subclass. A table view delegate provides views for table rows and columns, and supports functionality such as column reordering and resizing and row selection. To learn more about table views, see NSTableView.

## Topics

### Providing views for rows and columns

func tableView(NSTableView, viewFor: NSTableColumn?, row: Int) -> NSView?

Asks the delegate for a view to display the specified row and column.

func tableView(NSTableView, rowViewForRow: Int) -> NSTableRowView?

Asks the delegate for a view to display the specified row.

### Notification of row views being added or removed

func tableView(NSTableView, didAdd: NSTableRowView, forRow: Int)

Tells the delegate that a row view was added at the specified row.

func tableView(NSTableView, didRemove: NSTableRowView, forRow: Int)

Tells the delegate that a row view was removed from the table at the specified row.

### Grouping rows

func tableView(NSTableView, isGroupRow: Int) -> Bool

Returns whether the specified row is a group row.

### Providing cells for rows and columns

func tableView(NSTableView, willDisplayCell: Any, for: NSTableColumn?, row: Int)

Tells the delegate that the table view will display the specified cell at the specified row and column.

func tableView(NSTableView, dataCellFor: NSTableColumn?, row: Int) -> NSCell?

Asks the delegate for a custom data cell for the specified row and column.

func tableView(NSTableView, shouldShowCellExpansionFor: NSTableColumn?, row: Int) -> Bool

Asks the delegate if an expansion tooltip should be displayed for a specific row and column.

func tableView(NSTableView, toolTipFor: NSCell, rect: NSRectPointer, tableColumn: NSTableColumn?, row: Int, mouseLocation: NSPoint) -> String

Asks the delegate for a string to display in a tooltip for the specified cell in the column and row.

### Editing cells

func tableView(NSTableView, shouldEdit: NSTableColumn?, row: Int) -> Bool

Asks the delegate if the cell at the specified row and column can be edited.

### Setting row and column size

func tableView(NSTableView, heightOfRow: Int) -> CGFloat

Asks the delegate for the height of the specified row.

func tableView(NSTableView, sizeToFitWidthOfColumn: Int) -> CGFloat

Asks the delegate to provide custom sizing behavior when a column’s resize divider is double clicked.

### Selecting rows

func selectionShouldChange(in: NSTableView) -> Bool

Asks the delegate if the user is allowed to change the selection.

func tableView(NSTableView, shouldSelectRow: Int) -> Bool

Asks the delegate if the table view should allow selection of the specified row.

func tableView(NSTableView, selectionIndexesForProposedSelection: IndexSet) -> IndexSet

Asks the delegate to accept or reject the proposed selection.

func tableView(NSTableView, shouldSelect: NSTableColumn?) -> Bool

Asks the delegate whether the specified table column can be selected.

func tableViewSelectionIsChanging(Notification)

Tells the delegate that the table view’s selection is in the process of changing.

func tableViewSelectionDidChange(Notification)

Tells the delegate that the table view’s selection has changed.

func tableView(NSTableView, shouldTypeSelectFor: NSEvent, withCurrentSearch: String?) -> Bool

Asks the delegate to allow or deny type select for the specified event and current search string.

func tableView(NSTableView, typeSelectStringFor: NSTableColumn?, row: Int) -> String?

Asks the delegate to provide an alternative text value used for type selection for the specified row and column.

func tableView(NSTableView, nextTypeSelectMatchFromRow: Int, toRow: Int, for: String) -> Int

Asks the delegate for the row within the specified search range that matches the specified string.

### Moving and resizing columns

func tableView(NSTableView, shouldReorderColumn: Int, toColumn: Int) -> Bool

Asks the delegate to allow or prohibit the specified column to be dragged to a new location.

func tableView(NSTableView, didDrag: NSTableColumn)

Tells the delegate that the specified table column was dragged.

func tableViewColumnDidMove(Notification)

Tells the delegate that a table column was moved by user action.

func tableViewColumnDidResize(Notification)

Tells the delegate that a table column was resized.

### Responding to mouse events

func tableView(NSTableView, didClick: NSTableColumn)

Tells the delegate that the mouse button was clicked in the specified table column, but the column was not dragged.

func tableView(NSTableView, mouseDownInHeaderOf: NSTableColumn)

Tells the delegate that the mouse button was clicked in the specified table column’s header.

func tableView(NSTableView, shouldTrackCell: NSCell, for: NSTableColumn?, row: Int) -> Bool

Asks the delegate whether the specified cell should be tracked.

### Enabling table row actions

func tableView(NSTableView, rowActionsForRow: Int, edge: NSTableView.RowActionEdge) -> [NSTableViewRowAction]

Asks the delegate to provide an array of row actions to be attached to the specified edge of a table row and displayed when the user swipes horizontally across the row.

### Showing and hiding columns

func tableView(NSTableView, userCanChangeVisibilityOf: NSTableColumn) -> Bool

Asks the delegate to verify that the user can change the given column’s visibility.

func tableView(NSTableView, userDidChangeVisibilityOf: [NSTableColumn])

Tells the delegate that the user changed the visibility of one or more table columns.

## Relationships

### Inherits From

- NSControlTextEditingDelegate
- NSObjectProtocol

## See Also

### Management

protocol NSTableViewDataSource

A set of methods that a table view uses to provide data to a table view and to allow the editing of the table view’s data source object.

class NSTableViewDiffableDataSource

The object you use to manage data and provide items for a table view.

