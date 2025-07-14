

- AppKit
- NSMatrix
-  selectedCells 

Instance Property

# selectedCells

An array containing all of the matrix’s highlighted cells plus its selected cell.

macOS

``` source
@MainActor
var selectedCells: [NSCell] { get }
```

## Discussion

See the class description for a discussion of the selected cell.

As an alternative to using setSelectionFrom(_:to:anchor:highlight:) for programmatically making discontiguous selections of cells in a matrix, you could first set the single selected cell and then set subsequent cells to be highlighted; afterwards you can access selectedCells to obtain the selection of cells.

## See Also

### Related Documentation

var isHighlighted: Bool

A Boolean value indicating whether the cell has a highlighted appearance.

### Finding Cells

var selectedColumn: Int

The column number of the selected cell.

var selectedRow: Int

The row number of the selected cell.

func cell(atRow: Int, column: Int) -> NSCell?

Returns the cell at the specified row and column.

func cell(withTag: Int) -> NSCell?

Searches the receiver and returns the last cell matching the specified tag.

var cells: [NSCell]

An array containing the cells of the matrix.

