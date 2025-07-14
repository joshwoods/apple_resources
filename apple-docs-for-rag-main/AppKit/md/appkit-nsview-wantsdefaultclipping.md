

- AppKit
- NSView
-  wantsDefaultClipping 

Instance Property

# wantsDefaultClipping

A Boolean value indicating whether AppKit’s default clipping behavior is in effect.

macOS

``` source
@MainActor
var wantsDefaultClipping: Bool { get }
```

## Return Value

true if the default clipping is in effect, false otherwise. By default, this method returns true.

## Discussion

The default value of this property is true. When the value of this property is true, AppKit sets the current clipping region to the bounds of the view prior to calling that view’s draw(_:) method. Subclasses may override this property and return false to suppress this default clipping behavior. You might do this to avoid the cost of setting up, enforcing, and cleaning up the clipping path. If you do change the value to false, you are responsible for doing your own clipping or constraining drawing appropriately. Failure to do so could the view to corrupt the contents of other views in the window.

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

func bitmapImageRepForCachingDisplay(in: NSRect) -> NSBitmapImageRep?

Returns a bitmap-representation object suitable for caching the specified portion of the view.

func cacheDisplay(in: NSRect, to: NSBitmapImageRep)

Draws the specified area of the view, and its descendants, into a provided bitmap-representation object.

enum NSBorderType

These constants specify the type of a view’s border.

