

- AppKit
- NSMatrix
-  sort(using:context:) 

Instance Method

# sort(using:context:)

Sorts the receiver’s cells in ascending order as defined by the specified comparison function.

macOS

``` source
@MainActor
func sort(
    using compare: (Any, Any, UnsafeMutableRawPointer?) -> Int,
    context: UnsafeMutableRawPointer?
)
```

## Parameters 

`compare`  

The function to use when comparing cells. The comparison function is used to compare two elements at a time and should return `NSOrderedAscending` if the first element is smaller than the second, `NSOrderedDescending` if the first element is larger than the second, and `NSOrderedSame` if the elements are equal.

`context`  

Context passed to the comparison function as its third argument, each time its called. This allows the comparison to be based on some outside parameter, such as whether character sorting is case-sensitive or case-insensitive.

## See Also

### Related Documentation

func sort((Any, Any, UnsafeMutableRawPointer?) -> Int, context: UnsafeMutableRawPointer?)

Sorts the receiver in ascending order as defined by the comparison function \`compare\`.

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

