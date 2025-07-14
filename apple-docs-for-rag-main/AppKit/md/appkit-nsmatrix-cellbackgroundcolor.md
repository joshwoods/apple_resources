

- AppKit
- NSMatrix
-  cellBackgroundColor 

Instance Property

# cellBackgroundColor

The background color of the matrix’s cells.

macOS

``` source
@NSCopying @MainActor
var cellBackgroundColor: NSColor? { get set }
```

## Discussion

The value of this property is the background color used to fill the space behind non-opaque cells. The default background color is the color returned by the NSColor method controlColor.

## See Also

### Modifying Graphics Attributes

var backgroundColor: NSColor

The background color of the matrix (the space between the cells).

var drawsBackground: Bool

A Boolean that indicates whether the matrix draws its background.

var drawsCellBackground: Bool

A Boolean that indicates whether the matrix draws the background within each of its cells.

