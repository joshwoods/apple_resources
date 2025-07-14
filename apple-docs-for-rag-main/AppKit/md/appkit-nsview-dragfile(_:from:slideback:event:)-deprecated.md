

- AppKit
- NSView
-  dragFile(\_:from:slideBack:event:) Deprecated

Instance Method

# dragFile(\_:from:slideBack:event:)

Initiates a dragging operation from the view, allowing the user to drag a file icon to any application that has window or view objects that accept files.

macOS 10.0–10.13Deprecated

``` source
@MainActor
func dragFile(
    _ filename: String,
    from rect: NSRect,
    slideBack flag: Bool,
    event: NSEvent
) -> Bool
```

Deprecated

Use beginDraggingSession(with:event:source:) instead.

## Parameters 

`filename`  

A string that specifies the absolute path for the file that is dragged.

`rect`  

A rectangle that describes the position of the icon in the view’s coordinate system.

`flag`  

A Boolean that indicates whether the icon being dragged should slide back to its position in the view if the file isn’t accepted. The icon slides back to `aRect` if `slideBack` is true, the file is not accepted by the dragging destination, and the user has not disabled icon animation; otherwise it simply disappears.

`event`  

The mouse-down event object from which to initiate the drag operation. In particular, its mouse location is used for the offset of the icon being dragged.

## Return Value

true if the view successfully initiates the dragging operation (which doesn’t necessarily mean the dragging operation concluded successfully). Otherwise, this method returns false.

## Discussion

This method must be invoked only within an implementation of the mouseDown(with:) method.

See the NSDraggingSource, NSDraggingInfo, and NSDraggingDestination protocol specifications for more information on dragging operations.

## See Also

### Related Documentation

func shouldDelayWindowOrdering(for: NSEvent) -> Bool

Allows the user to drag objects from the view without activating the app or moving the window of the view forward, possibly obscuring the destination.

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

func setUpGState()

Overridden by subclasses to (re)initialize the view’s graphics state object.

Deprecated

func renewGState()

Invalidates the view’s graphics state object, if it has one.

Deprecated

func releaseGState()

Frees the view’s graphics state object, if it has one.

Deprecated

func dragPromisedFiles(ofTypes: [String], from: NSRect, source: Any, slideBack: Bool, event: NSEvent) -> Bool

Initiates a dragging operation from the view, allowing the user to drag one or more promised files (or directories) into any application that has window or view objects that accept promised file data.

Deprecated

