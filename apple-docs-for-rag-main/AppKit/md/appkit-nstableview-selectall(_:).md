

- AppKit
- NSTableView
-  selectAll(\_:) 

Instance Method

# selectAll(\_:)

Selects all rows or all columns, according to whether rows or columns were most recently selected.

macOS

``` source
@MainActor
func selectAll(_ sender: Any?)
```

## Parameters 

`sender`  

Typically the object that sent the message.

## Discussion

If the table allows multiple selection, this action method selects all rows or all columns, according to whether rows or columns were most recently selected. If nothing has been recently selected, this method selects all rows. If this table doesn’t allow multiple selection, this method does nothing.

If the selection does change, this method posts selectionDidChangeNotification to the default notification center.

As a target-action method, selectAll(_:) checks with the delegate before changing the selection.

## See Also

### Related Documentation

var allowsMultipleSelection: Bool

A Boolean value indicating whether the table view allows the user to select more than one column or row at a time.

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

func deselectRow(Int)

Deselects the row at the specified index if it’s selected.

var numberOfSelectedRows: Int

The number of selected rows.

func isRowSelected(Int) -> Bool

Returns a Boolean value that indicates whether the row at the specified index is selected.

func deselectAll(Any?)

Deselects all selected rows or columns if empty selection is allowed; otherwise does nothing.

