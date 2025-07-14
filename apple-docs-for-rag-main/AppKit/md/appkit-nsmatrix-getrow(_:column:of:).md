

- AppKit
- NSMatrix
-  getRow(\_:column:of:) 

Instance Method

# getRow(\_:column:of:)

Searches the receiver for the specified cell and returns the row and column of the cell

macOS

``` source
@MainActor
func getRow(
    _ row: UnsafeMutablePointer,
    column col: UnsafeMutablePointer,
    of cell: NSCell
) -> Bool
```

## Parameters 

`row`  

On return, the row in which the cell is located.

`col`  

On return, the column in which the cell is located.

`cell`  

The cell to locate within the matrix.

## Return Value

true if the cell is one of the cells in the receiver, false otherwise.

## Discussion

.

## See Also

### Finding Matrix Coordinates

func getRow(UnsafeMutablePointer&lt;Int>, column: UnsafeMutablePointer&lt;Int>, for: NSPoint) -> Bool

Indicates whether the specified point lies within one of the cells of the matrix and returns the location of the cell within which the point lies.

