

- AppKit
- NSMatrix
-  cells 

Instance Property

# cells

An array containing the cells of the matrix.

macOS

``` source
@MainActor
var cells: [NSCell] { get }
```

## Discussion

The cells in the array are row-ordered; that is, the first row of cells appears first in the array, followed by the second row, and so forth.

## See Also

### Finding Cells

var selectedCells: [NSCell]

An array containing all of the matrix’s highlighted cells plus its selected cell.

var selectedColumn: Int

The column number of the selected cell.

var selectedRow: Int

The row number of the selected cell.

func cell(atRow: Int, column: Int) -> NSCell?

Returns the cell at the specified row and column.

func cell(withTag: Int) -> NSCell?

Searches the receiver and returns the last cell matching the specified tag.

