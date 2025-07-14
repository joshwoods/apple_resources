

- AppKit
- NSTableView
-  setFocusedColumn(\_:) Deprecated

Instance Method

# setFocusedColumn(\_:)

Sets the currently focused column to the specified index.

macOS 10.6–10.10Deprecated

``` source
@MainActor
func setFocusedColumn(_ focusedColumn: Int)
```

Deprecated

Use a view-based table view and make a particular view the first responder to focus it.

## Parameters 

`focusedColumn`  

The index of the column to focus, or -1 if there should be no focused column.

## Discussion

This method will redisplay the previously focused column and (if required) the new `focusedColumn`.

The focused column has a focus ring drawn around the selectedRow that intersects with `focusedColumn`.

You should not override this method.

Note

This method is not applicable for NSView-based table views.

## See Also

### Deprecated Methods

func focusedColumn() -> Int

Returns the currently focused column.

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

