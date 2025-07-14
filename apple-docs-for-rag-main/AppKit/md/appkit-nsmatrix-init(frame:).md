

- AppKit
- NSMatrix
-  init(frame:) 

Initializer

# init(frame:)

Initializes a newly allocated matrix with the specified frame.

macOS

``` source
@MainActor
convenience init(frame frameRect: NSRect)
```

## Parameters 

`frameRect`  

The frame with which to initialize the matrix.

## Return Value

The NSMatrix, initialized with default parameters. The new NSMatrix contains no rows or columns. The default mode is `NSRadioModeMatrix`. The default cell class is NSActionCell.

## Discussion

.

## See Also

### Related Documentation

Matrix Programming Guide

### Initializing an NSMatrix Object

init(frame: NSRect, mode: NSMatrix.Mode, cellClass: AnyClass?, numberOfRows: Int, numberOfColumns: Int)

Initializes and returns a newly allocated matrix of the specified size using cells of the given class.

init(frame: NSRect, mode: NSMatrix.Mode, prototype: NSCell, numberOfRows: Int, numberOfColumns: Int)

Initializes and returns a newly allocated matrix of the specified size using the given cell as a prototype.

