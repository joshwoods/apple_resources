

- AppKit
- NSView
-  clipsToBounds 

Instance Property

# clipsToBounds

A Boolean value that indicates whether the view, and its subviews, confine their drawing areas to the bounds of the view.

macOS 10.9+

``` source
@MainActor
var clipsToBounds: Bool { get set }
```

## Discussion

Setting this value to true causes the view, and its subviews, to clip themselves to the bounds of the view. Setting it to false prevents views and subviews whose frames extend beyond the visible bounds of the view from clipping themselves. A value of false has no effect on hitTest(_:) but does affect visibleRect, as well as the area drawn inside draw(_:).

By default this value is false. In macOS 13 and earlier, the default value is true.

Because of this change in default value, views built on macOS 13 and earlier may require layout adjustments such as the following on newer versions of macOS:

- Showing or hiding UI elements by setting a parent’s frame size to zero. To hide a view hierarchy by shrinking the parent view, or positioning a child view outside a parent’s bounds, set the clipsToBounds property of the parent view to true. Alternatively, set isHidden to true on the parent view instead.

- Filling the `dirtyRect` of a view inside draw(_:). It’s a common practice to set the background color on a view by calling setFill() on a background color and then calling fill(using:) on the `dirtyRect` parameter passed into an override of draw(_:). Because the `dirtyRect` now extends outside your view’s bounds, call fill(using:) on the view’s bounds instead of the `dirtyRect`, or set the view’s clipsToBounds to true.

- Differentiating a view’s bounds from its `dirtyRect`. Use the `dirtyRect` parameter passed to draw(_:) to determine what to draw, not where to draw it. Use the view’s bounds to determine the layout of what your view draws.

## See Also

### Drawing the View’s Content

func updateLayer()

Updates the view’s content by modifying its underlying layer.

func draw(NSRect)

Overridden by subclasses to draw the view’s image within the specified rectangle.

var canDrawConcurrently: Bool

A Boolean value indicating whether the view can draw its contents on a background thread.

var visibleRect: NSRect

The portion of the view that isn’t clipped by its superviews.

func getRectsBeingDrawn(UnsafeMutablePointer&lt;UnsafePointer&lt;NSRect>?>?, count: UnsafeMutablePointer&lt;Int>?)

Returns by indirection a list of nonoverlapping rectangles that define the area the view is being asked to draw in draw(_:).

func needsToDraw(NSRect) -> Bool

Returns a Boolean value indicating whether the specified rectangle intersects any part of the area that the view is being asked to draw.

var wantsDefaultClipping: Bool

A Boolean value indicating whether AppKit’s default clipping behavior is in effect.

func bitmapImageRepForCachingDisplay(in: NSRect) -> NSBitmapImageRep?

Returns a bitmap-representation object suitable for caching the specified portion of the view.

func cacheDisplay(in: NSRect, to: NSBitmapImageRep)

Draws the specified area of the view, and its descendants, into a provided bitmap-representation object.

enum NSBorderType

These constants specify the type of a view’s border.

