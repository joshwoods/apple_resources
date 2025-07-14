

- AppKit
- NSView
-  bitmapImageRepForCachingDisplay(in:) 

Instance Method

# bitmapImageRepForCachingDisplay(in:)

Returns a bitmap-representation object suitable for caching the specified portion of the view.

macOS

``` source
@MainActor
func bitmapImageRepForCachingDisplay(in rect: NSRect) -> NSBitmapImageRep?
```

## Parameters 

`rect`  

A rectangle defining the area of the view to be cached.

## Return Value

An autoreleased NSBitmapImageRep object or `nil` if the object could not be created.

## Discussion

Passing the visible rectangle of the view (`[self visibleRect]`) returns a bitmap suitable for caching the current contents of the view, including all of its descendants.

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

func cacheDisplay(in: NSRect, to: NSBitmapImageRep)

Draws the specified area of the view, and its descendants, into a provided bitmap-representation object.

enum NSBorderType

These constants specify the type of a view’s border.

