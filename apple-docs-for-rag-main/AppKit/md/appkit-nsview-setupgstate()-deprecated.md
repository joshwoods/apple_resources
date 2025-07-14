

- AppKit
- NSView
-  setUpGState() Deprecated

Instance Method

# setUpGState()

Overridden by subclasses to (re)initialize the view’s graphics state object.

macOS 10.0–10.10Deprecated

``` source
@MainActor
func setUpGState()
```

Deprecated

Manage graphics state using an NSGraphicsContext object.

## Discussion

This method is automatically invoked when the graphics state object created using allocateGState() needs to be initialized. The default implementation does nothing. Your subclass can override it to set the current font, line width, or any other graphics state parameter except coordinate transformations and the clipping path—these are established by the frame and bounds rectangles and by methods such as scaleUnitSquare(to:) and translateOrigin(to:). Note that `drawRect:` can further transform the coordinate system and clipping path for whatever temporary effects it needs.

## See Also

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

func scroll(NSRect, by: NSSize)

Copies the visible portion of the view’s rendered image within a region and lays that portion down again at a specified offset .

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

