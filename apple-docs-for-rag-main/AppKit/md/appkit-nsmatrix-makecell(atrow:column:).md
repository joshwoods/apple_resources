

- AppKit
- NSMatrix
-  makeCell(atRow:column:) 

Instance Method

# makeCell(atRow:column:)

Creates a new cell at the location specified by the given row and column in the receiver.

macOS

``` source
@MainActor
func makeCell(
    atRow row: Int,
    column col: Int
) -> NSCell
```

## Parameters 

`row`  

The row in which to create the new cell.

`col`  

The column in which to create the new cell.

## Return Value

The newly created cell.

## Discussion

If the receiver has a prototype cell, it’s copied to create the new cell. If not, and if the receiver has a cell class set, it allocates and initializes (with `init`) an instance of that class. If the receiver hasn’t had either a prototype cell or a cell class set, NSMatrix creates an NSActionCell.

Your code should never invoke this method directly; it’s used by addRow() and other methods when a cell must be created. It may be overridden to provide more specific initialization of cells.

## See Also

### Related Documentation

var prototype: NSCell?

The prototype cell that’s copied whenever the matrix creates a new cell.

var cellClass: AnyClass

The subclass of NSCell that the matrix uses when creating new (empty) cells.

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

var numberOfColumns: Int

The number of columns in the matrix.

var numberOfRows: Int

The number of rows in the matrix.

func putCell(NSCell, atRow: Int, column: Int)

Replaces the cell at the specified row and column with the new cell.

