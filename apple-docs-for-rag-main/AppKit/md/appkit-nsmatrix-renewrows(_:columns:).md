

- AppKit
- NSMatrix
-  renewRows(\_:columns:) 

Instance Method

# renewRows(\_:columns:)

Changes the number of rows and columns in the receiver.

macOS

``` source
@MainActor
func renewRows(
    _ newRows: Int,
    columns newCols: Int
)
```

## Parameters 

`newRows`  

The new number of rows in the matrix.

`newCols`  

The new number of columns in the matrix.

## Discussion

This method uses the same cells as before, creating new cells only if the new size is larger; it never frees cells. It doesn’t redisplay the receiver. Your code should normally send sizeToCells() after invoking this method to resize the receiver so it fits the changed cell arrangement. This method deselects all cells in the receiver.

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

