

- AppKit
- NSMatrix
-  cell(withTag:) 

Instance Method

# cell(withTag:)

Searches the receiver and returns the last cell matching the specified tag.

macOS

``` source
@MainActor
func cell(withTag tag: Int) -> NSCell?
```

## Parameters 

`tag`  

The tag of the cell to return.

## Return Value

The last (when viewing the matrix as a row-ordered array) NSCell object that has a tag matching `anInt`, or `nil` if no such cell exists

## See Also

### Related Documentation

func selectCell(withTag: Int) -> Bool

Selects the last cell with the given tag.

var tag: Int

Returns the receiver’s tag.

### Finding Cells

var selectedCells: [NSCell]

An array containing all of the matrix’s highlighted cells plus its selected cell.

var selectedColumn: Int

The column number of the selected cell.

var selectedRow: Int

The row number of the selected cell.

func cell(atRow: Int, column: Int) -> NSCell?

Returns the cell at the specified row and column.

var cells: [NSCell]

An array containing the cells of the matrix.

