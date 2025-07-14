

- AppKit
- NSMatrix
-  isAutoscroll 

Instance Property

# isAutoscroll

A Boolean that indicates whether the receiver is automatically scrolled.

macOS

``` source
@MainActor
var isAutoscroll: Bool { get set }
```

## Discussion

When the value of this property is true, the matrix, if it is in a scrolling view, is automatically scrolled whenever the cursor is dragged outside the matrix after a mouse-down event within its bounds.

## See Also

### Scrolling Cells in the Matrix

func setScrollable(Bool)

Specifies whether the cells in the matrix are scrollable.

func scrollCellToVisible(atRow: Int, column: Int)

Scrolls the receiver so the specified cell is visible.

