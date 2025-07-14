

- AppKit
- NSBrowser
-  scrollColumnToVisible(\_:) 

Instance Method

# scrollColumnToVisible(\_:)

Scrolls to make the specified column visible.

macOS

``` source
@MainActor
func scrollColumnToVisible(_ column: Int)
```

## Parameters 

`column`  

The index of the column to scroll to.

## See Also

### Scrolling

var hasHorizontalScroller: Bool

A Boolean that indicates whether the browser has a horizontal scroller.

func scrollColumnsLeft(by: Int)

Scrolls columns left by the specified number of columns.

func scrollColumnsRight(by: Int)

Scrolls columns right by the specified number of columns.

func scrollRowToVisible(Int, inColumn: Int)

Scrolls the specified row to be visible within the specified column.

