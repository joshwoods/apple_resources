

- AppKit
- NSView
-  canDrawConcurrently 

Instance Property

# canDrawConcurrently

A Boolean value indicating whether the view can draw its contents on a background thread.

macOS 10.6+

``` source
@MainActor
var canDrawConcurrently: Bool { get set }
```

## Discussion

If your view’s draw(_:) implementation can draw safely on a background thread, set this property to true. Doing so gives AppKit the ability to run your view’s drawing code off the app’s main thread, which can improve performance. The view’s window must also have its allowsConcurrentViewDrawing property set to true (the default) for threaded view drawing to occur.

## See Also

### Drawing the View’s Content

func updateLayer()

Updates the view’s content by modifying its underlying layer.

func draw(NSRect)

Overridden by subclasses to draw the view’s image within the specified rectangle.

var clipsToBounds: Bool

A Boolean value that indicates whether the view, and its subviews, confine their drawing areas to the bounds of the view.

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

