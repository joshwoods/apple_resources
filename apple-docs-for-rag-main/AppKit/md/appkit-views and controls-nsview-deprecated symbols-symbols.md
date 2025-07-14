

- AppKit
- Views and Controls
- NSView
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Review unsupported symbols and their replacements.

## Topics

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

func dragFile(String, from: NSRect, slideBack: Bool, event: NSEvent) -> Bool

Initiates a dragging operation from the view, allowing the user to drag a file icon to any application that has window or view objects that accept files.

Deprecated

func dragPromisedFiles(ofTypes: [String], from: NSRect, source: Any, slideBack: Bool, event: NSEvent) -> Bool

Initiates a dragging operation from the view, allowing the user to drag one or more promised files (or directories) into any application that has window or view objects that accept promised file data.

Deprecated

### Properties

var wantsExtendedDynamicRangeOpenGLSurface: BoolDeprecated

var acceptsTouchEvents: Bool

A Boolean value indicating whether the view accepts touch events.

Deprecated

var canDraw: Bool

A Boolean value indicating whether drawing commands will produce any results.

Deprecated

var wantsBestResolutionOpenGLSurface: Bool

A Boolean value indicating whether the view wants an OpenGL backing surface with a resolution greater than 1 pixel per point.

Deprecated

### Notifications

class let globalFrameDidChangeNotification: NSNotification.Name

Posted whenever an `NSView` object that has attached surfaces (that is, `NSOpenGLContext` objects) moves to a different screen, or other cases where the `NSOpenGLContext` object needs to be updated.

Deprecated

