

- AppKit
- NSTableView
-  cornerView 

Instance Property

# cornerView

The view used to draw the area to the right of the column headers and above the vertical scroller of the enclosing scroll view.

macOS

``` source
@MainActor
var cornerView: NSView? { get set }
```

## Return Value

The view used to draw the area to the right of the column headers and above the vertical scroller of the enclosing `NSScrollView` object.

## Discussion

The default corner view draws a bezeled rectangle using a blank NSTableHeaderCell object, but you can replace it with a custom view that displays an image, or with a control that can handle mouse events, such as a Select All button. Your custom corner view should be as wide as a vertical NSScroller object and as tall as the header view of the table view.

## See Also

### Setting Auxiliary Views

var headerView: NSTableHeaderView?

The view object used to draw headers over columns.

