

- AppKit
- NSMatrix
-  keyCell 

Instance Property

# keyCell

The cell that will be clicked when the user presses the Space bar.

macOS

``` source
@MainActor
var keyCell: NSCell? { get set }
```

## See Also

### Related Documentation

var tabKeyTraversesCells: Bool

A Boolean that indicates whether pressing the Tab key advances the key cell to the next selectable cell.

### Selecting and Deselecting Cells

func selectCell(atRow: Int, column: Int)

Selects the cell at the specified row and column within the receiver.

func selectCell(withTag: Int) -> Bool

Selects the last cell with the given tag.

func selectAll(Any?)

Selects and highlights all cells in the receiver.

func setSelectionFrom(Int, to: Int, anchor: Int, highlight: Bool)

Programmatically selects a range of cells.

func deselectAllCells()

Deselects all cells in the receiver and, if necessary, redisplays the receiver.

func deselectSelectedCell()

Deselects the selected cell or cells.

