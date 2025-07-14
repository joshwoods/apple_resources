

- AppKit
- NSMatrix
-  cellSize 

Instance Property

# cellSize

The size of each cell in the matrix.

macOS

``` source
@MainActor
var cellSize: NSSize { get set }
```

## Discussion

This value corresponds to both the width and height of each cell, because all cells in an NSMatrix are the same size.

## See Also

### Laying Out the Cells of the Matrix

func addColumn()

Adds a new column of cells to the right of the last column.

func addColumn(with: [NSCell])

Adds a new column of cells to the right of the last column, using the given cells.

func addRow()

Adds a new row of cells below the last row.

func addRow(with: [NSCell])

Adds a new row of cells below the last row, using the specified cells.

func cellFrame(atRow: Int, column: Int) -> NSRect

Returns the frame rectangle of the cell that would be drawn at the specified location.

func getNumberOfRows(UnsafeMutablePointer&lt;Int>?, columns: UnsafeMutablePointer&lt;Int>?)

Obtains the number of rows and columns in the receiver.

func insertColumn(Int)

Inserts a new column of cells at the specified location. .

func insertColumn(Int, with: [NSCell]?)

Inserts a new column of cells before the specified column, using the given cells.

func insertRow(Int)

Inserts a new row of cells before the specified row.

func insertRow(Int, with: [NSCell]?)

Inserts a new row of cells before the specified row, using the given cells.

var intercellSpacing: NSSize

The vertical and horizontal spacing between cells in the matrix.

func makeCell(atRow: Int, column: Int) -> NSCell

Creates a new cell at the location specified by the given row and column in the receiver.

var numberOfColumns: Int

The number of columns in the matrix.

var numberOfRows: Int

The number of rows in the matrix.

func putCell(NSCell, atRow: Int, column: Int)

Replaces the cell at the specified row and column with the new cell.

