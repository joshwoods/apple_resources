

- AppKit
- NSTableView
-  performClickOnCell(atColumn:row:) Deprecated

Instance Method

# performClickOnCell(atColumn:row:)

Performs a click action on the cell at the specified row and column.

macOS 10.6–10.10Deprecated

``` source
@MainActor
func performClickOnCell(
    atColumn column: Int,
    row: Int
)
```

Deprecated

Use a view-based table view and use the view to handle user interactions.

## Parameters 

`column`  

The column of the cell.

`row`  

The row of the cell.

## Discussion

Acquires the NSTableView, copies it, invokes performClick(_:) or performClick(withFrame:in:) (if the cell is an NSPopUpButtonCell), and then updates the data source, if required. This method does not do any checks to see if the cell is enabled.

Note

This method is only available to NSCell-based table views.

## See Also

### Deprecated Methods

func focusedColumn() -> Int

Returns the currently focused column.

Deprecated

func setFocusedColumn(Int)

Sets the currently focused column to the specified index.

Deprecated

func shouldFocusCell(NSCell, atColumn: Int, row: Int) -> Bool

Returns whether the fully prepared cell at the specified row and column can be made the focused cell.

Deprecated

func preparedCell(atColumn: Int, row: Int) -> NSCell?

Returns the fully prepared cell that the table view will use for drawing or processing of the specified row and column.

Deprecated

