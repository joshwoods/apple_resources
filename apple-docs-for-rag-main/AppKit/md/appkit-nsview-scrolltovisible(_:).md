

- AppKit
- NSView
-  scrollToVisible(\_:) 

Instance Method

# scrollToVisible(\_:)

Scrolls the view’s closest ancestor NSClipView object the minimum distance needed so a specified region of the view becomes visible in the clip view.

macOS

``` source
@MainActor
func scrollToVisible(_ rect: NSRect) -> Bool
```

## Parameters 

`rect`  

The rectangle to be made visible in the clip view.

## Discussion

true if any scrolling is performed; otherwise returns false.

## See Also

### Related Documentation

func scroll(to: NSPoint)

Changes the origin of the clip view’s bounds rectangle to `newOrigin`.

func isDescendant(of: NSView) -> Bool

Returns a Boolean value that indicates whether the view is a subview of the specified view.

### Scrolling the View

func prepareContent(in: NSRect)

Prepares the overdraw region for drawing.

var preparedContentRect: NSRect

The portion of the view that has been rendered and is available for responsive scrolling.

func scroll(NSPoint)

Scrolls the view’s closest ancestor NSClipView object so a point in the view lies at the origin of the clip view’s bounds rectangle.

func autoscroll(with: NSEvent) -> Bool

Scrolls the view’s closest ancestor NSClipView object proportionally to the distance of an event that occurs outside of it.

func adjustScroll(NSRect) -> NSRect

Overridden by subclasses to modify a given rectangle, returning the altered rectangle.

var enclosingScrollView: NSScrollView?

The nearest ancestor scroll view that contains the current view.

func scroll(NSClipView, to: NSPoint)

Notifies the superview of a clip view that the clip view needs to reset the origin of its bounds rectangle.

func reflectScrolledClipView(NSClipView)

Notifies a clip view’s superview that either the clip view’s bounds rectangle or the document view’s frame rectangle has changed, and that any indicators of the scroll position need to be adjusted.

class var isCompatibleWithResponsiveScrolling: Bool

A Boolean value that indicates whether views support responsive scrolling.

