

- AppKit
- NSMatrix
-  prototype 

Instance Property

# prototype

The prototype cell that’s copied whenever the matrix creates a new cell.

macOS

``` source
@NSCopying @MainActor
var prototype: NSCell? { get set }
```

## Discussion

When the value of this property is `nil`, there is no prototype cell.

## See Also

### Related Documentation

init(frame: NSRect, mode: NSMatrix.Mode, prototype: NSCell, numberOfRows: Int, numberOfColumns: Int)

Initializes and returns a newly allocated matrix of the specified size using the given cell as a prototype.

func makeCell(atRow: Int, column: Int) -> NSCell

Creates a new cell at the location specified by the given row and column in the receiver.

### Managing the Cell Class

var cellClass: AnyClass

The subclass of NSCell that the matrix uses when creating new (empty) cells.

