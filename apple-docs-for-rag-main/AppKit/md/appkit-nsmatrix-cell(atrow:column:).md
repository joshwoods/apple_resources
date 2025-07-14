

- AppKit
- NSMatrix
-  cell(atRow:column:) 

Instance Method

# cell(atRow:column:)

Returns the cell at the specified row and column.

macOS

``` source
@MainActor
func cell(
    atRow row: Int,
    column col: Int
) -> NSCell?
```

## Parameters 

`row`  

The number of the row containing the cell to return.

`col`  

The number of the column containing the cell to return.

## Return Value

The NSCell object at the specified row and column location specified, or `nil` if either `row` or `column` is outside the bounds of the receiver.

## See Also

### Related Documentation

func getRow(UnsafeMutablePointer&lt;Int>, column: UnsafeMutablePointer&lt;Int>, of: NSCell) -> Bool

Searches the receiver for the specified cell and returns the row and column of the cell

### Finding Cells

var selectedCells: [NSCell]

An array containing all of the matrix’s highlighted cells plus its selected cell.

var selectedColumn: Int

The column number of the selected cell.

var selectedRow: Int

The row number of the selected cell.

func cell(withTag: Int) -> NSCell?

Searches the receiver and returns the last cell matching the specified tag.

var cells: [NSCell]

An array containing the cells of the matrix.

