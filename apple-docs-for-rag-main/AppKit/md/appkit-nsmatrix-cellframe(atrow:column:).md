

- AppKit
- NSMatrix
-  cellFrame(atRow:column:) 

Instance Method

# cellFrame(atRow:column:)

Returns the frame rectangle of the cell that would be drawn at the specified location.

macOS

``` source
@MainActor
func cellFrame(
    atRow row: Int,
    column col: Int
) -> NSRect
```

## Parameters 

`row`  

The row of the cell.

`col`  

The column of the cell.

## Return Value

The frame rectangle of the cell (whether or not the specified cell actually exists).

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

var cellSize: NSSize

The size of each cell in the matrix.

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

