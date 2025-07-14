

- AppKit
- NSView
-  getRectsBeingDrawn(\_:count:) 

Instance Method

# getRectsBeingDrawn(\_:count:)

Returns by indirection a list of nonoverlapping rectangles that define the area the view is being asked to draw in draw(_:).

macOS

``` source
@MainActor
func getRectsBeingDrawn(
    _ rects: UnsafeMutablePointer?>?,
    count: UnsafeMutablePointer?
)
```

## Parameters 

`rects`  

On return, contains a list of nonoverlapping rectangles defining areas to be drawn in. The rectangles returned in `rects` are in the coordinate space of the view.

`count`  

On return, the number of rectangles in the `rects` list.

## Discussion

An implementation of draw(_:) can use this information to test whether objects or regions within the view intersect with the rectangles in the list, and thereby avoid unnecessary drawing that would be completely clipped away.

The needsToDraw(_:) method gives you a convenient way to test individual objects for intersection with the area being drawn in draw(_:). However, you may want to retrieve and directly inspect the rectangle list if this is a more efficient way to perform intersection testing.

You should send this message only from within a draw(_:) implementation. The `aRect` parameter of draw(_:) is the rectangle enclosing the returned list of rectangles; you can use it in an initial pass to reject objects that are clearly outside the area to be drawn.

## See Also

### Drawing the View’s Content

func updateLayer()

Updates the view’s content by modifying its underlying layer.

func draw(NSRect)

Overridden by subclasses to draw the view’s image within the specified rectangle.

var clipsToBounds: Bool

A Boolean value that indicates whether the view, and its subviews, confine their drawing areas to the bounds of the view.

var canDrawConcurrently: Bool

A Boolean value indicating whether the view can draw its contents on a background thread.

var visibleRect: NSRect

The portion of the view that isn’t clipped by its superviews.

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

