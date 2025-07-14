

- AppKit
- NSTableView
-  selectRowIndexes(\_:byExtendingSelection:) 

Instance Method

# selectRowIndexes(\_:byExtendingSelection:)

Sets the row selection using `indexes` extending the selection if specified.

macOS

``` source
@MainActor
func selectRowIndexes(
    _ indexes: IndexSet,
    byExtendingSelection extend: Bool
)
```

## Parameters 

`indexes`  

The indexes to select.

`extend`  

true if the selection should be extended, false if the current selection should be changed.

## Discussion

Replaces the deprecated selectRow:byExtendingSelection: method.

## See Also

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

func selectAll(Any?)

Selects all rows or all columns, according to whether rows or columns were most recently selected.

func deselectAll(Any?)

Deselects all selected rows or columns if empty selection is allowed; otherwise does nothing.

