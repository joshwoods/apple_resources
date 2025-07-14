

- AppKit
- NSView
-  scroll(\_:by:) Deprecated

Instance Method

# scroll(\_:by:)

Copies the visible portion of the view’s rendered image within a region and lays that portion down again at a specified offset .

macOS 10.0–10.14Deprecated

``` source
@MainActor
func scroll(
    _ rect: NSRect,
    by delta: NSSize
)
```

Deprecated

Use NSScrollView to achieve scrolling views.

## Parameters 

`rect`  

A rectangle defining a region of the view.

`delta`  

A `NSSize` structure that specifies an offset from `aRect`’s origin.

## Discussion

This method is useful during scrolling or translation of the coordinate system to efficiently move as much of the view’s rendered image as possible without requiring it to be redrawn, following these steps:

1.  Invoke scroll(_:by:) to copy the rendered image.

2.  Move the view object’s origin or scroll it within its superview.

3.  Calculate the newly exposed rectangles and either set the needsDisplay property to true or call setNeedsDisplay(_:) to draw them.

You should rarely need to use this method, however. The scroll(_:), scrollToVisible(_:), and autoscroll(with:) methods automatically perform optimized scrolling.

## See Also

### Related Documentation

func setBoundsOrigin(NSPoint)

Sets the origin of the view’s bounds rectangle to a specified point.

func translateOrigin(to: NSPoint)

Translates the view’s coordinate system so that its origin moves to a new location.

### Methods

func lockFocus()

Locks the focus on the view, so subsequent commands take effect in the view’s window and coordinate system.

Deprecated

func lockFocusIfCanDraw() -> Bool

Locks the focus to the view atomically if the `canDraw` method returns true and returns the value of `canDraw`.

Deprecated

func lockFocusIfCanDraw(in: NSGraphicsContext) -> Bool

Locks the focus to the view atomically if drawing can occur in the specified graphics context.

Deprecated

func unlockFocus()

Unlocks focus from the current view.

Deprecated

func shouldDrawColor() -> Bool

Returns a Boolean value indicating whether the view is being drawn to an environment that supports color.

Deprecated

func allocateGState()

Causes the view to maintain a private graphics state object, which encapsulates all parameters of the graphics environment.

Deprecated

func gState() -> Int

Returns the identifier for the view’s graphics state object, or 0 if the view doesn’t have a graphics state object.

Deprecated

func setUpGState()

Overridden by subclasses to (re)initialize the view’s graphics state object.

Deprecated

func renewGState()

Invalidates the view’s graphics state object, if it has one.

Deprecated

func releaseGState()

Frees the view’s graphics state object, if it has one.

Deprecated

func dragFile(String, from: NSRect, slideBack: Bool, event: NSEvent) -> Bool

Initiates a dragging operation from the view, allowing the user to drag a file icon to any application that has window or view objects that accept files.

Deprecated

func dragPromisedFiles(ofTypes: [String], from: NSRect, source: Any, slideBack: Bool, event: NSEvent) -> Bool

Initiates a dragging operation from the view, allowing the user to drag one or more promised files (or directories) into any application that has window or view objects that accept promised file data.

Deprecated

