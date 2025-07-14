

- AppKit
- NSView
-  displayIgnoringOpacity(\_:in:) 

Instance Method

# displayIgnoringOpacity(\_:in:)

Causes the view and its descendants to be redrawn to the specified graphics context.

macOS

``` source
@MainActor
func displayIgnoringOpacity(
    _ rect: NSRect,
    in context: NSGraphicsContext
)
```

## Parameters 

`rect`  

A rectangle defining the region of the view to be redrawn. It should be specified in the coordinate system of the view.

`context`  

The graphics context in which drawing will occur. See the discussion below for more about this parameter.

## Discussion

Acts as display(), but confines drawing to `aRect`. This method initiates drawing with the view, even if the view is not opaque. Appropriate scaling factors for the view are obtained from `context`.

If the `context` parameter represents the context for the window containing the view, then all of the necessary transformations are applied. This includes the application of the view’s bounds and frame transforms along with any transforms it inherited from its ancestors. In this situation, the view is also marked as no longer needing an update for the specified rectangle.

If `context` specifies any other graphics context, then only the view’s bounds transform is applied. This means that drawing is not constrained to the view’s visible rectangle. It also means that any dirty rectangles are not cleared, since they are not being redrawn to the window.

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

