

- AppKit
- NSView
-  translateRectsNeedingDisplay(in:by:) 

Instance Method

# translateRectsNeedingDisplay(in:by:)

Translates the display rectangles by the specified delta.

macOS 10.5+

``` source
@MainActor
func translateRectsNeedingDisplay(
    in clipRect: NSRect,
    by delta: NSSize
)
```

## Parameters 

`clipRect`  

A rectangle defining the region of the view, typically the view’s bounds.

`delta`  

A NSSize structure that specifies an offset from aRect’s origin.

## Discussion

This method performs the shifting of dirty rectangles that an equivalent scroll(_:by:) operation would cause, without performing the actual scroll operation. It is only useful in very rare cases where a view implements its own low-level scrolling mechanics.

This method:

1.  Collects the receiving view’s dirty rectangles.

2.  Clears all dirty rectangles in the intersection of `clipRect` and the view’s bounds.

3.  Shifts the retrieved rectangles by the `delta` offset.

4.  Clips the result to the intersection of `clipRect` and the view’s bounds

5.  Marks the resultant rectangles as needing display.

The developer must ensure that `clipRect` and `delta` are pixel-aligned in order to guarantee correct drawing. See Transforming View Coordinates To and From Base Space for a description of how to pixel-align view coordinates.

## See Also

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

var isOpaque: Bool

A Boolean value indicating whether the view fills its frame rectangle with opaque content.

func viewWillDraw()

Informs the view that it’s required to draw content.

