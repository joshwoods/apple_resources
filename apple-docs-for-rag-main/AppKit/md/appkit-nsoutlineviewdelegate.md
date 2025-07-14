

- AppKit
-  NSOutlineViewDelegate 

Protocol

# NSOutlineViewDelegate

A set of optional methods implemented by delegates of NSOutlineView objects.

macOS

``` source
protocol NSOutlineViewDelegate : NSControlTextEditingDelegate
```

## Topics

### Expanding and Collapsing the Outline

func outlineView(NSOutlineView, shouldExpandItem: Any) -> Bool

Returns a Boolean value that indicates whether the outline view should expand a given item.

func outlineView(NSOutlineView, shouldCollapseItem: Any) -> Bool

Returns a Boolean value that indicates whether the outline view should collapse a given item.

### Supporting Type Select

func outlineView(NSOutlineView, typeSelectStringFor: NSTableColumn?, item: Any) -> String?

Returns the string that is used for type selection for a given column and item.

func outlineView(NSOutlineView, nextTypeSelectMatchFromItem: Any, toItem: Any, for: String) -> Any?

Returns the first item that matches the searchString from within the range of startItem to endItem

func outlineView(NSOutlineView, shouldTypeSelectFor: NSEvent, withCurrentSearch: String?) -> Bool

Returns a Boolean value that indicates whether type select should proceed for a given event and search string.

### Working with Tooltips

func outlineView(NSOutlineView, toolTipFor: NSCell, rect: NSRectPointer, tableColumn: NSTableColumn?, item: Any, mouseLocation: NSPoint) -> String

When the cursor pauses over a given cell, the value returned from this method is displayed in a tooltip.

### Handling Selection

func outlineView(NSOutlineView, shouldSelect: NSTableColumn?) -> Bool

Returns a Boolean value that indicates whether the outline view should select a given table column.

func outlineView(NSOutlineView, shouldSelectItem: Any) -> Bool

Returns a Boolean value that indicates whether the outline view should select a given item.

func outlineView(NSOutlineView, selectionIndexesForProposedSelection: IndexSet) -> IndexSet

Invoked to allow the delegate to modify the proposed selection.

func selectionShouldChange(in: NSOutlineView) -> Bool

Returns a Boolean value that indicates whether the outline view should change its selection.

func outlineViewSelectionIsChanging(Notification)

Invoked when `notification` is posted—that is, whenever the outline view’s selection changes.

func outlineViewSelectionDidChange(Notification)

Invoked when the selection did change notification is posted—that is, immediately after the outline view’s selection has changed.

### Displaying Cells

func outlineView(NSOutlineView, willDisplayCell: Any, for: NSTableColumn?, item: Any)

Informs the delegate that the cell specified by the column and item will be displayed.

func outlineView(NSOutlineView, willDisplayOutlineCell: Any, for: NSTableColumn?, item: Any)

Informs the delegate that an outline view is about to display a cell used to draw the expansion symbol.

func outlineView(NSOutlineView, dataCellFor: NSTableColumn?, item: Any) -> NSCell?

Returns the cell to use in a given column for a given item.

func outlineView(NSOutlineView, shouldShowOutlineCellForItem: Any) -> Bool

Returns whether the specified item should display the outline cell (the disclosure triangle).

func outlineView(NSOutlineView, shouldShowCellExpansionFor: NSTableColumn?, item: Any) -> Bool

Invoked to allow the delegate to control cell expansion for a specific column and item.

### Moving and Resizing Columns

func outlineView(NSOutlineView, shouldReorderColumn: Int, toColumn: Int) -> Bool

Sent to the delegate to allow or prohibit the specified column to be dragged to a new location.

### Working with the Outline Column

func outlineViewColumnDidMove(Notification)

Invoked whenever the user moves a column in the outline view.

func outlineViewColumnDidResize(Notification)

Invoked whenever the user resizes a column in the outline view.

func outlineViewItemWillExpand(Notification)

Invoked when `notification` is posted—that is, whenever the user is about to expand an item in the outline view.

func outlineViewItemDidExpand(Notification)

Invoked when `notification` is posted—that is, whenever the user expands an item in the outline view.

func outlineViewItemWillCollapse(Notification)

Invoked when `notification` is posted—that is, whenever the user is about to collapse an item in the outline view.

func outlineViewItemDidCollapse(Notification)

Invoked when the did collapse notification is posted—that is, whenever the user collapses an item in the outline view.

### Editing Items

func outlineView(NSOutlineView, shouldEdit: NSTableColumn?, item: Any) -> Bool

Returns a Boolean value that indicates whether the outline view should allow editing of a given item in a given table column.

### Working with Table Columns

func outlineView(NSOutlineView, mouseDownInHeaderOf: NSTableColumn)

Sent to the delegate whenever the mouse button is clicked in `outlineView` while the cursor is in a column header `tableColumn`.

func outlineView(NSOutlineView, didClick: NSTableColumn)

Sent at the time the mouse button subsequently goes up in `outlineView` and `tableColumn` has been “clicked” without having been dragged anywhere.

func outlineView(NSOutlineView, didDrag: NSTableColumn)

Sent at the time the mouse button goes up in `outlineView` and `tableColumn` has been dragged during the time the mouse button was down.

### Customizing Column and Row Sizes

func outlineView(NSOutlineView, heightOfRowByItem: Any) -> CGFloat

Returns the height in points of the row containing `item`.

func outlineView(NSOutlineView, sizeToFitWidthOfColumn: Int) -> CGFloat

Invoked to allow the delegate to provide custom sizing behavior when a column’s resize divider is double clicked.

### Customizing Tint Color

func outlineView(NSOutlineView, tintConfigurationForItem: Any) -> NSTintConfiguration?

Customizes an item’s tinting behavior.

class NSTintConfiguration

An object that gives you the ability to choose from system-provided tinting behaviors.

### Customizing Tracking Support

func outlineView(NSOutlineView, shouldTrackCell: NSCell, for: NSTableColumn?, item: Any) -> Bool

Returns a Boolean value that indicates whether a given cell should be tracked.

### Grouping Rows

func outlineView(NSOutlineView, isGroupItem: Any) -> Bool

Returns a Boolean that indicates whether a given row should be drawn in the “group row” style.

### Working with NSView-Based Outline Views

func outlineView(NSOutlineView, didAdd: NSTableRowView, forRow: Int)

Implemented to know when a new row view is added to the table.

func outlineView(NSOutlineView, didRemove: NSTableRowView, forRow: Int)

Implemented to know when a row view is removed from the table

func outlineView(NSOutlineView, rowViewForItem: Any) -> NSTableRowView?

implement this method to return a custom `NSTableRowView` for a particular item.

func outlineView(NSOutlineView, viewFor: NSTableColumn?, item: Any) -> NSView?

Implemented to return the view used to display the specified item and column.

### Changing Visibility

func outlineView(NSOutlineView, userCanChangeVisibilityOf: NSTableColumn) -> Bool

func outlineView(NSOutlineView, userDidChangeVisibilityOf: [NSTableColumn])

## Relationships

### Inherits From

- NSControlTextEditingDelegate
- NSObjectProtocol

## See Also

### Management

protocol NSOutlineViewDataSource

A set of methods that an outline view calls to retrieve data and information about it from the data source delegate, and—optionally—to update data values.

