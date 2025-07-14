

- AppKit
- NSMatrix
-  sort(using:) 

Instance Method

# sort(using:)

Sorts the receiver’s cells in ascending order as defined by the comparison method.

macOS

``` source
@MainActor
func sort(using comparator: Selector)
```

## Parameters 

`comparator`  

The comparison method.

## Discussion

The comparator message is sent to each object in the matrix and has as its single argument another object in the array. The comparison method is used to compare two elements at a time and should return `NSOrderedAscending` if the receiver is smaller than the argument, `NSOrderedDescending` if the receiver is larger than the argument, and `NSOrderedSame` if they are equal.

## See Also

### Related Documentation

func sort(using: Selector)

Sorts the receiver in ascending order, as determined by the comparison method specified by a given selector.

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

