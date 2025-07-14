

- AppKit
- NSTableHeaderCell
-  drawSortIndicator(withFrame:in:ascending:priority:) 

Instance Method

# drawSortIndicator(withFrame:in:ascending:priority:)

Draws a sorting indicator given a cell frame contained inside a view.

macOS

``` source
@MainActor
func drawSortIndicator(
    withFrame cellFrame: NSRect,
    in controlView: NSView,
    ascending: Bool,
    priority: Int
)
```

## Parameters 

`cellFrame`  

The cell frame.

`controlView`  

The control view.

`ascending`  

If YES the sort indicator is drawn as ascending; otherwise it is drawn as descending.

`priority`  

If `priority` is 0, this is the primary sort indicator.

## Discussion

Override this method to customize the sorting user interface.

## See Also

### Related Documentation

Table View Programming Guide for Mac

### Drawing Sorting Indicators

func sortIndicatorRect(forBounds: NSRect) -> NSRect

Returns the location to display the sorting indicator given `theRect`.

