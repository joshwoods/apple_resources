

- AppKit
- NSTableView
-  focusedColumn() Deprecated

Instance Method

# focusedColumn()

Returns the currently focused column.

macOS 10.5–10.10Deprecated

``` source
@MainActor
func focusedColumn() -> Int
```

Deprecated

Use a view-based table view and observe the window’s first responder.

## Return Value

The index of the column, or -1 if there is no focused column

## Discussion

The focus interaction will always be on the selectedRow of the table. If the selectedRow is a full width cell, then `focusedColumn` will return `1` when focused.

Note

This method is not applicable for NSView-based table views. Instead, the view that has focus will be the firstResponder.

## See Also

### Deprecated Methods

func setFocusedColumn(Int)

Sets the currently focused column to the specified index.

Deprecated

func shouldFocusCell(NSCell, atColumn: Int, row: Int) -> Bool

Returns whether the fully prepared cell at the specified row and column can be made the focused cell.

Deprecated

func performClickOnCell(atColumn: Int, row: Int)

Performs a click action on the cell at the specified row and column.

Deprecated

func preparedCell(atColumn: Int, row: Int) -> NSCell?

Returns the fully prepared cell that the table view will use for drawing or processing of the specified row and column.

Deprecated

