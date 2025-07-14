

- AppKit
- NSView
-  preparedContentRect 

Instance Property

# preparedContentRect

The portion of the view that has been rendered and is available for responsive scrolling.

macOS 10.9+

``` source
@MainActor
var preparedContentRect: NSRect { get set }
```

## Discussion

During responsive scrolling, this property specifies the portion of the view that has been rendered and is ready to scroll. This rectangle always includes the visible portion of the view and may also include nonvisible portions that have been rendered and cached.

Changing the value of this property alerts AppKit that it might need to generate new overdraw content. For example, setting the value to the current visible rectangle forces AppKit to throw away any cached overdraw content and regenerate it during the next idle period. Never assign a rectangle that is smaller than the visible rectangle.

## See Also

### Scrolling the View

func prepareContent(in: NSRect)

Prepares the overdraw region for drawing.

func scroll(NSPoint)

Scrolls the view’s closest ancestor NSClipView object so a point in the view lies at the origin of the clip view’s bounds rectangle.

func scrollToVisible(NSRect) -> Bool

Scrolls the view’s closest ancestor NSClipView object the minimum distance needed so a specified region of the view becomes visible in the clip view.

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

