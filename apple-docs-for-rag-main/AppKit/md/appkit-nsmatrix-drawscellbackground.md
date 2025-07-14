

- AppKit
- NSMatrix
-  drawsCellBackground 

Instance Property

# drawsCellBackground

A Boolean that indicates whether the matrix draws the background within each of its cells.

macOS

``` source
@MainActor
var drawsCellBackground: Bool { get set }
```

## Discussion

When the value of this property is true, the matrix draws the cell background.

## See Also

### Modifying Graphics Attributes

var backgroundColor: NSColor

The background color of the matrix (the space between the cells).

var cellBackgroundColor: NSColor?

The background color of the matrix’s cells.

var drawsBackground: Bool

A Boolean that indicates whether the matrix draws its background.

