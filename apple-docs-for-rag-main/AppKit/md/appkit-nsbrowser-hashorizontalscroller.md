

- AppKit
- NSBrowser
-  hasHorizontalScroller 

Instance Property

# hasHorizontalScroller

A Boolean that indicates whether the browser has a horizontal scroller.

macOS

``` source
@MainActor
var hasHorizontalScroller: Bool { get set }
```

## Discussion

When the value of this property is true, the browser uses an `NSScroller` object to scroll horizontally.

## See Also

### Scrolling

func scrollColumnToVisible(Int)

Scrolls to make the specified column visible.

func scrollColumnsLeft(by: Int)

Scrolls columns left by the specified number of columns.

func scrollColumnsRight(by: Int)

Scrolls columns right by the specified number of columns.

func scrollRowToVisible(Int, inColumn: Int)

Scrolls the specified row to be visible within the specified column.

