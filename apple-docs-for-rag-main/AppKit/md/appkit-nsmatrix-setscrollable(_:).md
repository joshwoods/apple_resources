

- AppKit
- NSMatrix
-  setScrollable(\_:) 

Instance Method

# setScrollable(\_:)

Specifies whether the cells in the matrix are scrollable.

macOS

``` source
@MainActor
func setScrollable(_ flag: Bool)
```

## Parameters 

`flag`  

true to make all the cells in the receiver scrollable, so the text they contain scrolls to remain in view if the user types past the edge of the cell. If `flag` is false, all cells are made nonscrolling. The prototype cell, if there is one, is also set accordingly

## See Also

### Related Documentation

var isScrollable: Bool

A Boolean value indicating whether excess text scrolls past the cell’s bounds.

var prototype: NSCell?

The prototype cell that’s copied whenever the matrix creates a new cell.

### Scrolling Cells in the Matrix

var isAutoscroll: Bool

A Boolean that indicates whether the receiver is automatically scrolled.

func scrollCellToVisible(atRow: Int, column: Int)

Scrolls the receiver so the specified cell is visible.

