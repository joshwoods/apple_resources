

- AppKit
- NSView
-  prepareContent(in:) 

Instance Method

# prepareContent(in:)

Prepares the overdraw region for drawing.

macOS 10.9+

``` source
@MainActor
func prepareContent(in rect: NSRect)
```

## Parameters 

`rect`  

The current overdraw region, specified in the view’s coordinate system. This rectangle includes the view’s visible rectangle plus any space surrounding the visible rectangle that represents the overdraw region.

## Discussion

During responsive scrolling, AppKit calls this method before asking your view to draw any content in the overdraw region. You can override this method in your own views and use it to prepare the content that is about to be drawn. For example, if your app defers the creation of subviews until they are scrolled into view, you would use this method to create them and add them to your view hierarchy.

Your implementation of this method must call `super` at some point. When calling `super`, you can extend the overdraw rectangle by passing a different rectangle for the `rect` parameter. For example, if you add a subview whose frame falls outside the current rectangle, you can grow the rectangle to include the entire frame of the subview.

AppKit may call this method multiple times to build up the current overdraw region slowly. Each time it calls the method, it extends the overdraw rectangle passed in the `rect` parameter. If you pass the same rectangle to `super` twice in succession, AppKit stops generating additional overdraw content. You can use this behavior to avoid generating more overdraw content than makes sense for your app. If the user scrolls the content, AppKit resets the current overdraw region and starts asking your app for content again. You can also reset the current overdraw region by assigning a value to the preparedContentRect property.

## See Also

### Scrolling the View

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

class var isCompatibleWithResponsiveScrolling: Bool

A Boolean value that indicates whether views support responsive scrolling.

