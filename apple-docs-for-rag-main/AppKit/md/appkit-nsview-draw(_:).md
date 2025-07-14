

- AppKit
- NSView
-  draw(\_:) 

Instance Method

# draw(\_:)

Overridden by subclasses to draw the view’s image within the specified rectangle.

macOS

``` source
@MainActor
func draw(_ dirtyRect: NSRect)
```

## Parameters 

`dirtyRect`  

A rectangle defining the portion of the view that requires redrawing. This rectangle usually represents the portion of the view that requires updating. When responsive scrolling is enabled, this rectangle can also represent a nonvisible portion of the view that AppKit wants to cache.

## Discussion

Use this method to draw the specified portion of your view’s content. Your implementation of this method should be as fast as possible and do as little work as possible. The `dirtyRect` parameter helps you achieve better performance by specifying the portion of the view that needs to be drawn. You should always limit drawing to the content inside this rectangle. For even better performance, you can call the getRectsBeingDrawn(_:count:) method and use the list of rectangles returned by that method to limit drawing even further. You can also use the needsToDraw(_:) method test whether objects in a particular rectangle need to be drawn.

The default implementation does nothing. Subclasses should override this method if they do custom drawing. Prior to calling this method, AppKit creates an appropriate drawing context and configures it for drawing to the view; you do not need to configure the drawing context yourself. If your app manages content using its layer object instead, use the updateLayer() method to update your layer instead of overriding this method.

If your custom view is a direct `NSView` subclass, you do not need to call `super`. For all other views, call `super` at some point in your implementation so that the parent class can perform any additional drawing.

Important

If the view’s isOpaque property is true, the view must completely fill the `dirtyRect` rectangle with opaque content.

For information about how to draw in your app, see Cocoa Drawing Guide.

## See Also

### Related Documentation

func shouldDrawColor() -> Bool

Returns a Boolean value indicating whether the view is being drawn to an environment that supports color.

Deprecated

func setNeedsDisplay(NSRect)

Marks the region of the view within the specified rectangle as needing display, increasing the view’s existing invalid region to include it.

func display()

Displays the view and all its subviews if possible, invoking each of the `NSView` methods lockFocus(), draw(_:), and unlockFocus() as necessary.

var isFlipped: Bool

A Boolean value indicating whether the view uses a flipped coordinate system.

### Drawing the View’s Content

func updateLayer()

Updates the view’s content by modifying its underlying layer.

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

func cacheDisplay(in: NSRect, to: NSBitmapImageRep)

Draws the specified area of the view, and its descendants, into a provided bitmap-representation object.

enum NSBorderType

These constants specify the type of a view’s border.

