

- AppKit
- NSTableHeaderCell
-  sortIndicatorRect(forBounds:) 

Instance Method

# sortIndicatorRect(forBounds:)

Returns the location to display the sorting indicator given `theRect`.

macOS

``` source
@MainActor
func sortIndicatorRect(forBounds rect: NSRect) -> NSRect
```

## Parameters 

`rect`  

A cell rectangle.

## Return Value

The rectangle within `theRect` that should contain the sorting indicator.

## See Also

### Drawing Sorting Indicators

func drawSortIndicator(withFrame: NSRect, in: NSView, ascending: Bool, priority: Int)

Draws a sorting indicator given a cell frame contained inside a view.

