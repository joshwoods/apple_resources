

- AppKit
- NSView
-  cacheDisplay(in:to:) 

Instance Method

# cacheDisplay(in:to:)

Draws the specified area of the view, and its descendants, into a provided bitmap-representation object.

macOS

``` source
@MainActor
func cacheDisplay(
    in rect: NSRect,
    to bitmapImageRep: NSBitmapImageRep
)
```

## Parameters 

`rect`  

A rectangle defining the region to be drawn into `bitmapImageRep`.

`bitmapImageRep`  

An NSBitmapImageRep object. For pixel-format compatibility, `bitmapImageRep` should have been obtained from bitmapImageRepForCachingDisplay(in:).

## Discussion

You are responsible for initializing the bitmap to the desired configuration before calling this method. However, once initialized, you can reuse the same bitmap multiple times to refresh the cached copy of your view’s contents.

The bitmap produced by this method is transparent (that is, has an alpha value of 0) wherever the view and its descendants do not draw any content.

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

func getRectsBeingDrawn(UnsafeMutablePointer&lt;UnsafePointer&lt;NSRect>?>?, count: UnsafeMutablePointer&lt;Int>?)

Returns by indirection a list of nonoverlapping rectangles that define the area the view is being asked to draw in draw(_:).

func needsToDraw(NSRect) -> Bool

Returns a Boolean value indicating whether the specified rectangle intersects any part of the area that the view is being asked to draw.

var wantsDefaultClipping: Bool

A Boolean value indicating whether AppKit’s default clipping behavior is in effect.

func bitmapImageRepForCachingDisplay(in: NSRect) -> NSBitmapImageRep?

Returns a bitmap-representation object suitable for caching the specified portion of the view.

enum NSBorderType

These constants specify the type of a view’s border.

