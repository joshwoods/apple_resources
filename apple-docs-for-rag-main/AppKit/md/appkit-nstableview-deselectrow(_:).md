

- AppKit
- NSTableView
-  deselectRow(\_:) 

Instance Method

# deselectRow(\_:)

Deselects the row at the specified index if it’s selected.

macOS

``` source
@MainActor
func deselectRow(_ row: Int)
```

## Parameters 

`row`  

The index of the row to deselect.

## Discussion

Deselects the row at `rowIndex` if it’s selected, regardless of whether empty selection is allowed.

If the selection does in fact change, posts selectionDidChangeNotification to the default notification center.

If the indicated row was the last row selected by the user, the row nearest it effectively becomes the last selected row. In case of a tie, priority is given to the row above.

This method doesn’t check with the delegate before changing the selection.

## See Also

### Related Documentation

var allowsEmptySelection: Bool

A Boolean value indicating whether the table view allows the user to select zero columns or rows.

### Selecting Columns and Rows

func selectColumnIndexes(IndexSet, byExtendingSelection: Bool)

Sets the column selection using `indexes` possibly extending the selection.

var selectedColumn: Int

The index of the last selected column (or the last column added to the selection).

var selectedColumnIndexes: IndexSet

An index set containing the indexes of the selected columns.

func deselectColumn(Int)

Deselects the column at the specified index if it’s selected.

var numberOfSelectedColumns: Int

The number of selected columns.

func isColumnSelected(Int) -> Bool

Returns a Boolean value that indicates whether the column at the specified index is selected.

func selectRowIndexes(IndexSet, byExtendingSelection: Bool)

Sets the row selection using `indexes` extending the selection if specified.

var selectedRow: Int

The index of the last selected row (or the last row added to the selection).

var selectedRowIndexes: IndexSet

An index set containing the indexes of the selected rows.

var numberOfSelectedRows: Int

The number of selected rows.

func isRowSelected(Int) -> Bool

Returns a Boolean value that indicates whether the row at the specified index is selected.

func selectAll(Any?)

Selects all rows or all columns, according to whether rows or columns were most recently selected.

func deselectAll(Any?)

Deselects all selected rows or columns if empty selection is allowed; otherwise does nothing.

