

- AppKit
- NSMatrix
-  selectAll(\_:) 

Instance Method

# selectAll(\_:)

Selects and highlights all cells in the receiver.

macOS

``` source
@MainActor
func selectAll(_ sender: Any?)
```

## Parameters 

`sender`  

This argument is ignored.

## Discussion

Editable text cells and disabled cells are not selected. The receiver is redisplayed.

If the selection mode is not NSMatrix.Mode.listModeMatrix, this method does nothing.

## See Also

### Related Documentation

func selectCell(NSCell)

Selects the specified cell and redraws the control as needed.

### Selecting and Deselecting Cells

func selectCell(atRow: Int, column: Int)

Selects the cell at the specified row and column within the receiver.

func selectCell(withTag: Int) -> Bool

Selects the last cell with the given tag.

var keyCell: NSCell?

The cell that will be clicked when the user presses the Space bar.

func setSelectionFrom(Int, to: Int, anchor: Int, highlight: Bool)

Programmatically selects a range of cells.

func deselectAllCells()

Deselects all cells in the receiver and, if necessary, redisplays the receiver.

func deselectSelectedCell()

Deselects the selected cell or cells.

