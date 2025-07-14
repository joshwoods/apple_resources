

- AppKit
- NSMatrix
-  selectedColumn 

Instance Property

# selectedColumn

The column number of the selected cell.

macOS

``` source
@MainActor
var selectedColumn: Int { get }
```

## Discussion

When the value of this property is `–1`, no cells are selected. If cells in multiple columns are selected, the value of this property is the number of the last (rightmost) column containing a selected cell.

## See Also

### Finding Cells

var selectedCells: [NSCell]

An array containing all of the matrix’s highlighted cells plus its selected cell.

var selectedRow: Int

The row number of the selected cell.

func cell(atRow: Int, column: Int) -> NSCell?

Returns the cell at the specified row and column.

func cell(withTag: Int) -> NSCell?

Searches the receiver and returns the last cell matching the specified tag.

var cells: [NSCell]

An array containing the cells of the matrix.

