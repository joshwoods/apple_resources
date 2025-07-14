

- AppKit
- NSView
-  isCompatibleWithResponsiveScrolling 

Type Property

# isCompatibleWithResponsiveScrolling

A Boolean value that indicates whether views support responsive scrolling.

macOS 10.9+

``` source
@MainActor
class var isCompatibleWithResponsiveScrolling: Bool { get }
```

## Discussion

When the value of this property is true, the view class supports responsive scrolling. AppKit enables responsive scrolling when the views involved in scrolling—the NSScrollView, NSClipView, and embedded document view—all have this property set to true. If you want to opt out of responsive scrolling, override this property and set it to false.

NSScrollView, NSClipView, and other view subclasses override this property and perform additional checks.

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

func adjustScroll(NSRect) -> NSRect

Overridden by subclasses to modify a given rectangle, returning the altered rectangle.

var enclosingScrollView: NSScrollView?

The nearest ancestor scroll view that contains the current view.

func scroll(NSClipView, to: NSPoint)

Notifies the superview of a clip view that the clip view needs to reset the origin of its bounds rectangle.

func reflectScrolledClipView(NSClipView)

Notifies a clip view’s superview that either the clip view’s bounds rectangle or the document view’s frame rectangle has changed, and that any indicators of the scroll position need to be adjusted.

