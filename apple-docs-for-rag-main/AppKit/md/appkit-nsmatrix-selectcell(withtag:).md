

- AppKit
- NSMatrix
-  selectCell(withTag:) 

Instance Method

# selectCell(withTag:)

Selects the last cell with the given tag.

macOS

``` source
@MainActor
func selectCell(withTag tag: Int) -> Bool
```

## Parameters 

`tag`  

The tag of the cell to select.

## Return Value

true if the receiver contains a cell whose tag matches `anInt`, or false if no such cell exists

## Discussion

If the matrix has at least one cell whose tag is equal to `anInt`, the last cell (when viewing the matrix as a row-ordered array) is selected. If the specified cell is an editable text cell, its text is selected.

## See Also

### Related Documentation

func cell(withTag: Int) -> NSCell?

Searches the receiver and returns the last cell matching the specified tag.

func selectCell(NSCell)

Selects the specified cell and redraws the control as needed.

### Selecting and Deselecting Cells

func selectCell(atRow: Int, column: Int)

Selects the cell at the specified row and column within the receiver.

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

