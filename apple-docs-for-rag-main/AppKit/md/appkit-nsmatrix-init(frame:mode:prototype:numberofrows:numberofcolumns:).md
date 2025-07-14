

- AppKit
- NSMatrix
-  init(frame:mode:prototype:numberOfRows:numberOfColumns:) 

Initializer

# init(frame:mode:prototype:numberOfRows:numberOfColumns:)

Initializes and returns a newly allocated matrix of the specified size using the given cell as a prototype.

macOS

``` source
@MainActor
init(
    frame frameRect: NSRect,
    mode: NSMatrix.Mode,
    prototype cell: NSCell,
    numberOfRows rowsHigh: Int,
    numberOfColumns colsWide: Int
)
```

## Parameters 

`frameRect`  

The matrix’s frame.

`mode`  

The tracking mode for the matrix; this can be one of the modes described in NSMatrix.Mode.

`cell`  

An instance of a subclass of NSCell, which the new matrix copies when it creates new cells.

`rowsHigh`  

The number of rows in the matrix.

`colsWide`  

The number of columns in the matrix.

## Discussion

This method is the designated initializer for matrices that add cells by copying an instance of an NSCell subclass.

## See Also

### Initializing an NSMatrix Object

convenience init(frame: NSRect)

Initializes a newly allocated matrix with the specified frame.

init(frame: NSRect, mode: NSMatrix.Mode, cellClass: AnyClass?, numberOfRows: Int, numberOfColumns: Int)

Initializes and returns a newly allocated matrix of the specified size using cells of the given class.

