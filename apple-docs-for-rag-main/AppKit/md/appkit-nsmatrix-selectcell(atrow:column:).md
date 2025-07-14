

- AppKit
- NSMatrix
-  selectCell(atRow:column:) 

Instance Method

# selectCell(atRow:column:)

Selects the cell at the specified row and column within the receiver.

macOS

``` source
@MainActor
func selectCell(
    atRow row: Int,
    column col: Int
)
```

## Parameters 

`row`  

The row of the cell to select.

`col`  

The column of the cell to select.

## Discussion

If the specified cell is an editable text cell, its text is selected. If either `row` or `column` is –1, then the current selection is cleared (unless the receiver is an `NSRadioModeMatrix` and doesn’t allow empty selection). This method redraws the affected cells.

## See Also

### Related Documentation

var mode: NSMatrix.Mode

The selection mode of the receiver.

func selectCell(NSCell)

Selects the specified cell and redraws the control as needed.

var allowsEmptySelection: Bool

A Boolean that indicates whether a radio-mode matrix supports an empty selection.

### Selecting and Deselecting Cells

func selectCell(withTag: Int) -> Bool

Selects the last cell with the given tag.

func selectAll(Any?)

Selects and highlights all cells in the receiver.

var keyCell: NSCell?

The cell that will be clicked when the user presses the Space bar.

func setSelectionFrom(Int, to: Int, anchor: Int, highlight: Bool)

Programmatically selects a range of cells.

func deselectAllCells()

Deselects all cells in the receiver and, if necessary, redisplays the receiver.

func deselectSelectedCell()

Deselects the selected cell or cells.

