

- AppKit
- NSView
-  display() 

Instance Method

# display()

Displays the view and all its subviews if possible, invoking each of the `NSView` methods lockFocus(), draw(_:), and unlockFocus() as necessary.

macOS

``` source
@MainActor
func display()
```

## Discussion

If the view isn’t opaque, this method backs up the view hierarchy to the first opaque ancestor, calculates the portion of the opaque ancestor covered by the view, and begins displaying from there.

## See Also

### Related Documentation

var canDraw: Bool

A Boolean value indicating whether drawing commands will produce any results.

Deprecated

var visibleRect: NSRect

The portion of the view that isn’t clipped by its superviews.

var opaqueAncestor: NSView?

The view’s closest opaque ancestor, which might be the view itself.

### Invalidating the View’s Content

func setNeedsDisplay(NSRect)

Marks the region of the view within the specified rectangle as needing display, increasing the view’s existing invalid region to include it.

var needsDisplay: Bool

A Boolean value that determines whether the view needs to be redrawn before being displayed.

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

