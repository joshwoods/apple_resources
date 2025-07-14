

- AppKit
- NSMatrix
-  getRow(\_:column:for:) 

Instance Method

# getRow(\_:column:for:)

Indicates whether the specified point lies within one of the cells of the matrix and returns the location of the cell within which the point lies.

macOS

``` source
@MainActor
func getRow(
    _ row: UnsafeMutablePointer,
    column col: UnsafeMutablePointer,
    for point: NSPoint
) -> Bool
```

## Parameters 

`row`  

On return, the row of the cell containing the specified point.

`col`  

On return, the column of the cell containing the specified point.

`point`  

The point to locate; this point should be in the coordinate system of the receiver.

## Return Value

true if the point lies within one of the cells in the receiver; false if the point falls outside the bounds of the receiver or lies within an intercell spacing.

## See Also

### Finding Matrix Coordinates

func getRow(UnsafeMutablePointer&lt;Int>, column: UnsafeMutablePointer&lt;Int>, of: NSCell) -> Bool

Searches the receiver for the specified cell and returns the row and column of the cell

