

- AppKit
- NSView
-  adjustScroll(\_:) 

Instance Method

# adjustScroll(\_:)

Overridden by subclasses to modify a given rectangle, returning the altered rectangle.

macOS

``` source
@MainActor
func adjustScroll(_ newVisible: NSRect) -> NSRect
```

## Parameters 

`newVisible`  

A rectangle that defines a region of the view.

## Discussion

NSClipView invokes this method to allow its document view to adjust its position during scrolling. For example, a custom view object that displays a table of data can adjust the origin of `newVisible` so rows or columns aren’t cut off by the edge of the enclosing NSClipView. The NSView implementation simply returns `newVisible`.

NSClipView only invokes this method during automatic or user controlled scrolling. Its scroll(to:) method doesn’t invoke this method, so you can still force a scroll to an arbitrary point.

## See Also

### Scrolling the View

func prepareContent(in: NSRect)

Prepares the overdraw region for drawing.

var preparedContentRect: NSRect

The portion of the view that has been rendered and is available for responsive scrolling.

func scroll(NSPoint)

Scrolls the view’s closest ancestor NSClipView object so a point in the view lies at the origin of the clip view’s bounds rectangle.

func scrollToVisible(NSRect) -> Bool

Scrolls the view’s closest ancestor NSClipView object the minimum distance needed so a specified region of the view becomes visible in the clip view.

func autoscroll(with: NSEvent) -> Bool

Scrolls the view’s closest ancestor NSClipView object proportionally to the distance of an event that occurs outside of it.

var enclosingScrollView: NSScrollView?

The nearest ancestor scroll view that contains the current view.

func scroll(NSClipView, to: NSPoint)

Notifies the superview of a clip view that the clip view needs to reset the origin of its bounds rectangle.

func reflectScrolledClipView(NSClipView)

Notifies a clip view’s superview that either the clip view’s bounds rectangle or the document view’s frame rectangle has changed, and that any indicators of the scroll position need to be adjusted.

class var isCompatibleWithResponsiveScrolling: Bool

A Boolean value that indicates whether views support responsive scrolling.

