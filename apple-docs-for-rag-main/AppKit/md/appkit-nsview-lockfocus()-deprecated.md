

- AppKit
- NSView
-  lockFocus() Deprecated

Instance Method

# lockFocus()

Locks the focus on the view, so subsequent commands take effect in the view’s window and coordinate system.

macOS 10.0–10.14Deprecated

``` source
@MainActor
func lockFocus()
```

Deprecated

Subclass the view and implement draw(_:) instead.

## Discussion

If you don’t use a `display` method to draw an `NSView` object, you must invoke lockFocus() before invoking methods that send commands to the window server, and must balance it with an unlockFocus() message when finished.

Hiding or miniaturizing a one-shot window causes the backing store for that window to be released. (A one-shot window frees its window device when the window is hidden and another is created when it’s returned to the screen.) If you don’t use the standard display mechanism to draw, you should use lockFocusIfCanDraw() rather than lockFocus() if there is a chance of drawing while the window is either miniaturized or hidden. This method throws an exception if the view is hidden or if drawing cannot happen for some other reason. To ensure that you can lock focus successfully, make sure the canDraw property is true; you can also call lockFocusIfCanDraw() instead and use the return value of that method to determine if focus was obtained successfully.

## See Also

### Related Documentation

func draw(NSRect)

Overridden by subclasses to draw the view’s image within the specified rectangle.

class var focusView: NSView?

The currently focused view object.

func display()

Displays the view and all its subviews if possible, invoking each of the `NSView` methods lockFocus(), draw(_:), and unlockFocus() as necessary.

### Methods

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

func dragFile(String, from: NSRect, slideBack: Bool, event: NSEvent) -> Bool

Initiates a dragging operation from the view, allowing the user to drag a file icon to any application that has window or view objects that accept files.

Deprecated

func dragPromisedFiles(ofTypes: [String], from: NSRect, source: Any, slideBack: Bool, event: NSEvent) -> Bool

Initiates a dragging operation from the view, allowing the user to drag one or more promised files (or directories) into any application that has window or view objects that accept promised file data.

Deprecated

