

- AppKit
- NSTableView
-  preparedCell(atColumn:row:) Deprecated

Instance Method

# preparedCell(atColumn:row:)

Returns the fully prepared cell that the table view will use for drawing or processing of the specified row and column.

macOS 10.5–10.10Deprecated

``` source
@MainActor
func preparedCell(
    atColumn column: Int,
    row: Int
) -> NSCell?
```

Deprecated

Use a view-based table view and the view(atColumn:row:makeIfNecessary:) method.

## Parameters 

`column`  

The index in the tableColumns array for which to return the appropriate cell.

`row`  

The row index for which to return the appropriate cell.

## Return Value

New NSCell subclass instance to use for the specified `row` and `column`. The value for the cell is correctly set, and the delegate method tableView(_:willDisplayCell:for:row:) will have been called.

## Discussion

You can override this method to do any additional cell set up that is required, or invoke it to retrieve a cell that has its contents configured for the specified `column` and `row`.

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

func performClickOnCell(atColumn: Int, row: Int)

Performs a click action on the cell at the specified row and column.

Deprecated

