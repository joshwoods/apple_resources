

- AppKit
- NSMatrix
-  init(frame:mode:cellClass:numberOfRows:numberOfColumns:) 

Initializer

# init(frame:mode:cellClass:numberOfRows:numberOfColumns:)

Initializes and returns a newly allocated matrix of the specified size using cells of the given class.

macOS

``` source
@MainActor
init(
    frame frameRect: NSRect,
    mode: NSMatrix.Mode,
    cellClass factoryId: AnyClass?,
    numberOfRows rowsHigh: Int,
    numberOfColumns colsWide: Int
)
```

## Parameters 

`frameRect`  

The matrix’s frame.

`mode`  

The tracking mode for the matrix; this can be one of the modes described in NSMatrix.Mode.

`factoryId`  

The class to use for any cells that the matrix creates and uses. This can be obtained by sending a `class` message to the desired subclass of NSCell.

`rowsHigh`  

The number of rows in the matrix.

`colsWide`  

The number of columns in the matrix.

## Return Value

The initialized instance of NSMatrix.

## Discussion

This method is the designated initializer for matrices that add cells by creating instances of an NSCell subclass.

## See Also

### Initializing an NSMatrix Object

convenience init(frame: NSRect)

Initializes a newly allocated matrix with the specified frame.

init(frame: NSRect, mode: NSMatrix.Mode, prototype: NSCell, numberOfRows: Int, numberOfColumns: Int)

Initializes and returns a newly allocated matrix of the specified size using the given cell as a prototype.

