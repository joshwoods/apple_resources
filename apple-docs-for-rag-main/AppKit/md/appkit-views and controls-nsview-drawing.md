

- AppKit
- Views and Controls
- NSView
-  Drawing 

API Collection

# Drawing

Draw the content of custom views and update that content when the view’s size or appearance changes.

## Topics

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

func cacheDisplay(in: NSRect, to: NSBitmapImageRep)

Draws the specified area of the view, and its descendants, into a provided bitmap-representation object.

enum NSBorderType

These constants specify the type of a view’s border.

### Drawing the View in Fullscreen Mode

func enterFullScreenMode(NSScreen, withOptions: [NSView.FullScreenModeOptionKey : Any]?) -> Bool

Sets the view to full screen mode.

func exitFullScreenMode(options: [NSView.FullScreenModeOptionKey : Any]?)

Instructs the view to exit full screen mode.

var isInFullScreenMode: Bool

A Boolean value indicating whether the view is in full screen mode.

struct FullScreenModeOptionKey

These constants are keys that you can use in the options dictionary in enterFullScreenMode(_:withOptions:) and exitFullScreenMode(options:).

### Invalidating the View’s Content

func setNeedsDisplay(NSRect)

Marks the region of the view within the specified rectangle as needing display, increasing the view’s existing invalid region to include it.

var needsDisplay: Bool

A Boolean value that determines whether the view needs to be redrawn before being displayed.

func display()

Displays the view and all its subviews if possible, invoking each of the `NSView` methods lockFocus(), draw(_:), and unlockFocus() as necessary.

func display(NSRect)

Acts as display(), but confining drawing to a rectangular region of the view.

func displayIgnoringOpacity(NSRect)

Displays the view but confines drawing to a specified region and does not back up to the first opaque ancestor—it simply causes the view and its descendants to execute their drawing code.

func displayIgnoringOpacity(NSRect, in: NSGraphicsContext)

Causes the view and its descendants to be redrawn to the specified graphics context.

func displayIfNeeded()

Displays the view and all its subviews if any part of the view has been marked as needing display.

func displayIfNeeded(NSRect)

Acts as displayIfNeeded(), confining drawing to a specified region of the view.

func displayIfNeededIgnoringOpacity()

Acts as displayIfNeeded(), except that this method doesn’t back up to the first opaque ancestor—it simply causes the view and its descendants to execute their drawing code.

func displayIfNeededIgnoringOpacity(NSRect)

Acts as displayIfNeeded(), but confining drawing to `aRect` and not backing up to the first opaque ancestor—it simply causes the view and its descendants to execute their drawing code.

func translateRectsNeedingDisplay(in: NSRect, by: NSSize)

Translates the display rectangles by the specified delta.

var isOpaque: Bool

A Boolean value indicating whether the view fills its frame rectangle with opaque content.

func viewWillDraw()

Informs the view that it’s required to draw content.

### Updating the View When Property Values Change

struct Invalidating

A property wrapper that notifies the system that a property value change has invalidated an aspect of the containing view.

protocol NSViewInvalidating

Implements a type of invalidation that can occur on a view that requires an update.

### Managing Live Resize

var inLiveResize: Bool

A Boolean value indicating whether the view is being rendered as part of a live resizing operation.

var preservesContentDuringLiveResize: Bool

A Boolean value indicating whether the view optimizes live-resize operations by preserving content that has not moved.

func getRectsExposedDuringLiveResize(UnsafeMutablePointer&lt;NSRect>, count: UnsafeMutablePointer&lt;Int>)

Returns a list of rectangles indicating the newly exposed areas of the view.

var rectPreservedDuringLiveResize: NSRect

The rectangle identifying the portion of your view that did not change during a live resize operation.

func viewWillStartLiveResize()

Informs the view of the start of a live resize—the user has started resizing the view.

func viewDidEndLiveResize()

Informs the view of the end of a live resize—the user has finished resizing the view.

## See Also

### Managing the view’s content

Layout

Specify the size and position your view relative to other nearby views using rules that update your view hierarchy automatically.

Printing

Create a printable version of your view’s content and handle pagination and printer-related behaviors.

