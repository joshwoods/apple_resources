

- AppKit
- NSView
-  visibleRect 

Instance Property

# visibleRect

The portion of the view that isn’t clipped by its superviews.

macOS

``` source
@MainActor
var visibleRect: NSRect { get }
```

## Discussion

Visibility, as reflected by this property, doesn’t account for whether other view or window objects overlap the current view or whether the current view is installed in a window at all. This value of this property is `NSZeroRect` if the current view is effectively hidden.

During a printing operation the visible rectangle is further clipped to the page being imaged.

clipsToBounds affects this property.

## See Also

### Related Documentation

var isHidden: Bool

A Boolean value indicating whether the view is hidden.

var documentVisibleRect: NSRect

The portion of the document view, in its own coordinate system, visible through the scroll view’s content view.

var documentVisibleRect: NSRect

The exposed rectangle of the clip view’s document view, in the document view’s own coordinate system.

var isVisible: Bool

A Boolean value that indicates whether the window is visible onscreen (even when it’s obscured by other windows).

### Drawing the View’s Content

func updateLayer()

Updates the view’s content by modifying its underlying layer.

func draw(NSRect)

Overridden by subclasses to draw the view’s image within the specified rectangle.

var clipsToBounds: Bool

A Boolean value that indicates whether the view, and its subviews, confine their drawing areas to the bounds of the view.

var canDrawConcurrently: Bool

A Boolean value indicating whether the view can draw its contents on a background thread.

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

