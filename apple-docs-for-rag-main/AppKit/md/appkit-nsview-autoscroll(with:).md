

- AppKit
- NSView
-  autoscroll(with:) 

Instance Method

# autoscroll(with:)

Scrolls the view’s closest ancestor NSClipView object proportionally to the distance of an event that occurs outside of it.

macOS

``` source
@MainActor
func autoscroll(with event: NSEvent) -> Bool
```

## Parameters 

`event`  

An event object whose location should be expressed in the window’s base coordinate system (which it normally is), not the receiving view’s.

## Return Value

Returns true if any scrolling is performed; otherwise returns false.

## Discussion

View objects that track mouse-dragged events can use this method to scroll automatically when the cursor is dragged outside of the NSClipView object. Repeated invocations of this method (with an appropriate delay) result in continual scrolling, even when the mouse doesn’t move.

## See Also

### Related Documentation

func isDescendant(of: NSView) -> Bool

Returns a Boolean value that indicates whether the view is a subview of the specified view.

func autoscroll(with: NSEvent) -> Bool

Scrolls the clip view proportionally to `theEvent`’s distance outside of it.

### Scrolling the View

func prepareContent(in: NSRect)

Prepares the overdraw region for drawing.

var preparedContentRect: NSRect

The portion of the view that has been rendered and is available for responsive scrolling.

func scroll(NSPoint)

Scrolls the view’s closest ancestor NSClipView object so a point in the view lies at the origin of the clip view’s bounds rectangle.

func scrollToVisible(NSRect) -> Bool

Scrolls the view’s closest ancestor NSClipView object the minimum distance needed so a specified region of the view becomes visible in the clip view.

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

