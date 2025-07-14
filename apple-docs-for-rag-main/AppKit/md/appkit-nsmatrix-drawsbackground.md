

- AppKit
- NSMatrix
-  drawsBackground 

Instance Property

# drawsBackground

A Boolean that indicates whether the matrix draws its background.

macOS

``` source
@MainActor
var drawsBackground: Bool { get set }
```

## Discussion

When the value of this property is true, the matrix draws its background (the space between the cells).

## See Also

### Modifying Graphics Attributes

var backgroundColor: NSColor

The background color of the matrix (the space between the cells).

var cellBackgroundColor: NSColor?

The background color of the matrix’s cells.

var drawsCellBackground: Bool

A Boolean that indicates whether the matrix draws the background within each of its cells.

