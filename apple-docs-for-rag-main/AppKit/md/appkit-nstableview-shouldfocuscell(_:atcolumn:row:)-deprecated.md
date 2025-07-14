

- AppKit
- NSTableView
-  shouldFocusCell(\_:atColumn:row:) Deprecated

Instance Method

# shouldFocusCell(\_:atColumn:row:)

Returns whether the fully prepared cell at the specified row and column can be made the focused cell.

macOS 10.6–10.10Deprecated

``` source
@MainActor
func shouldFocusCell(
    _ cell: NSCell,
    atColumn column: Int,
    row: Int
) -> Bool
```

Deprecated

Use a view-based table view and observe the window’s first responder.

## Parameters 

`cell`  

The prepared cell to be focused upon.

`column`  

The column of the cell.

`row`  

The row of the cell.

## Return Value

true if the cell can be made the focused cell, otherwise false.

## Discussion

By default, only cells that are enabled can be focused. In addition, if the cell is an NSTextFieldCell, it can only be focused if it is selectable or editable, and the table view delegate responds true to -tableView(_:shouldEdit:row:).

Subclasses can override this to further control which cells can and can’t be made focused.

Note

This method is only applicable to NSCell-based table views.

## See Also

### Deprecated Methods

func focusedColumn() -> Int

Returns the currently focused column.

Deprecated

func setFocusedColumn(Int)

Sets the currently focused column to the specified index.

Deprecated

func performClickOnCell(atColumn: Int, row: Int)

Performs a click action on the cell at the specified row and column.

Deprecated

func preparedCell(atColumn: Int, row: Int) -> NSCell?

Returns the fully prepared cell that the table view will use for drawing or processing of the specified row and column.

Deprecated

