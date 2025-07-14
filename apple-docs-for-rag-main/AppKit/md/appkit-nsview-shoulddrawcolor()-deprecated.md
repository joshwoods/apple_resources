

- AppKit
- NSView
-  shouldDrawColor() Deprecated

Instance Method

# shouldDrawColor()

Returns a Boolean value indicating whether the view is being drawn to an environment that supports color.

macOS 10.0–10.10Deprecated

``` source
@MainActor
func shouldDrawColor() -> Bool
```

Deprecated

The behavior offered by this method is no longer necessary.

## Return Value

true if the view’s window supports color drawing or false if it does not.

## Discussion

A view object can base its drawing behavior on the return value of this method to improve its appearance in grayscale windows. This method might return false when the view’s window does not store color information because the content is destined for a grayscale printer.

## See Also

### Related Documentation

func draw(NSRect)

Overridden by subclasses to draw the view’s image within the specified rectangle.

func canStoreColor() -> Bool

Indicates whether the window has a depth limit that allows it to store color values.

Deprecated

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

