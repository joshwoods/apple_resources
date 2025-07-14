

- AppKit
- NSTableView
-  isColumnSelected(\_:) 

Instance Method

# isColumnSelected(\_:)

Returns a Boolean value that indicates whether the column at the specified index is selected.

macOS

``` source
@MainActor
func isColumnSelected(_ column: Int) -> Bool
```

## Parameters 

`column`  

The index into the tableColumns array that represents the column to test.

## Return Value

true if the column at `columnIndex` is selected, otherwise false.

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

func selectAll(Any?)

Selects all rows or all columns, according to whether rows or columns were most recently selected.

func deselectAll(Any?)

Deselects all selected rows or columns if empty selection is allowed; otherwise does nothing.

