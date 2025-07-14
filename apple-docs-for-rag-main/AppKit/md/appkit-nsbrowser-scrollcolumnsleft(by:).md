

- AppKit
- NSBrowser
-  scrollColumnsLeft(by:) 

Instance Method

# scrollColumnsLeft(by:)

Scrolls columns left by the specified number of columns.

macOS

``` source
@MainActor
func scrollColumnsLeft(by shiftAmount: Int)
```

## Parameters 

`shiftAmount`  

The number of columns by which to scroll the browser.

## See Also

### Scrolling

var hasHorizontalScroller: Bool

A Boolean that indicates whether the browser has a horizontal scroller.

func scrollColumnToVisible(Int)

Scrolls to make the specified column visible.

func scrollColumnsRight(by: Int)

Scrolls columns right by the specified number of columns.

func scrollRowToVisible(Int, inColumn: Int)

Scrolls the specified row to be visible within the specified column.

