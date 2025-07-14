

- AppKit
- NSMatrix
-  scrollCellToVisible(atRow:column:) 

Instance Method

# scrollCellToVisible(atRow:column:)

Scrolls the receiver so the specified cell is visible.

macOS

``` source
@MainActor
func scrollCellToVisible(
    atRow row: Int,
    column col: Int
)
```

## Parameters 

`row`  

The row of the cell to make visible.

`col`  

The column of the cell to make visible.

## Discussion

This method scrolls if the receiver is in a scrolling view and `row` and `column` represent a valid cell within the receiver.

## See Also

### Related Documentation

func scrollToVisible(NSRect) -> Bool

Scrolls the view’s closest ancestor NSClipView object the minimum distance needed so a specified region of the view becomes visible in the clip view.

### Scrolling Cells in the Matrix

var isAutoscroll: Bool

A Boolean that indicates whether the receiver is automatically scrolled.

func setScrollable(Bool)

Specifies whether the cells in the matrix are scrollable.

