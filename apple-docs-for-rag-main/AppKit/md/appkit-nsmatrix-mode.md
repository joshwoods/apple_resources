

- AppKit
- NSMatrix
-  mode 

Instance Property

# mode

The selection mode of the receiver.

macOS

``` source
@MainActor
var mode: NSMatrix.Mode { get set }
```

## Discussion

See NSMatrix.Mode for possible values.

## See Also

### Related Documentation

init(frame: NSRect, mode: NSMatrix.Mode, cellClass: AnyClass?, numberOfRows: Int, numberOfColumns: Int)

Initializes and returns a newly allocated matrix of the specified size using cells of the given class.

init(frame: NSRect, mode: NSMatrix.Mode, prototype: NSCell, numberOfRows: Int, numberOfColumns: Int)

Initializes and returns a newly allocated matrix of the specified size using the given cell as a prototype.

### Configuring the Matrix Object

var allowsEmptySelection: Bool

A Boolean that indicates whether a radio-mode matrix supports an empty selection.

var isSelectionByRect: Bool

A Boolean that indicates whether the user can select a rectangle of cells in the receiver by dragging the cursor.

