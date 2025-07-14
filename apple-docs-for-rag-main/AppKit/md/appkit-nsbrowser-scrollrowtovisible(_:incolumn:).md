

- AppKit
- NSBrowser
-  scrollRowToVisible(\_:inColumn:) 

Instance Method

# scrollRowToVisible(\_:inColumn:)

Scrolls the specified row to be visible within the specified column.

macOS 10.6+

``` source
@MainActor
func scrollRowToVisible(
    _ row: Int,
    inColumn column: Int
)
```

## Parameters 

`row`  

The index of the row to scroll.

`column`  

The index of the column containing the row to scroll.

## Discussion

The row’s column will not be scrolled to visible via this method. To scroll the column to visible, use scrollColumnToVisible(_:).

## See Also

### Scrolling

var hasHorizontalScroller: Bool

A Boolean that indicates whether the browser has a horizontal scroller.

func scrollColumnToVisible(Int)

Scrolls to make the specified column visible.

func scrollColumnsLeft(by: Int)

Scrolls columns left by the specified number of columns.

func scrollColumnsRight(by: Int)

Scrolls columns right by the specified number of columns.

