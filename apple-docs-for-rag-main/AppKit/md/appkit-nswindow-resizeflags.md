

- AppKit
- NSWindow
-  resizeFlags 

Instance Property

# resizeFlags

The flags field of the event record for the mouse-down event that initiated the resizing session.

macOS

``` source
@MainActor
var resizeFlags: NSEvent.ModifierFlags { get }
```

## Discussion

The value of this property is a mask indicating which of the modifier keys was held down when the mouse-down event occurred. The flags are listed in NSEvent class’s modifierFlags method description. The property is valid only while the window is being resized.

You can use this property to constrain the direction or amount of resizing. Because of its limited validity, this property should only be accessed from within an implementation of the delegate method windowWillResize(_:to:).

## See Also

### Sizing Windows

var frame: NSRect

The window’s frame rectangle in screen coordinates, including the title bar.

func setFrameOrigin(NSPoint)

Positions the bottom-left corner of the window’s frame rectangle at a given point in screen coordinates.

func setFrameTopLeftPoint(NSPoint)

Positions the top-left corner of the window’s frame rectangle at a given point in screen coordinates.

func constrainFrameRect(NSRect, to: NSScreen?) -> NSRect

Modifies and returns a frame rectangle so that its top edge lies on a specific screen.

func cascadeTopLeft(from: NSPoint) -> NSPoint

Positions the window’s top-left to a given point.

func setFrame(NSRect, display: Bool)

Sets the origin and size of the window’s frame rectangle according to a given frame rectangle, thereby setting its position and size onscreen.

func setFrame(NSRect, display: Bool, animate: Bool)

Sets the origin and size of the window’s frame rectangle, with optional animation, according to a given frame rectangle, thereby setting its position and size onscreen.

func animationResizeTime(NSRect) -> TimeInterval

Specifies the duration of a smooth frame-size change.

var aspectRatio: NSSize

The window’s aspect ratio, which constrains the size of its frame rectangle to integral multiples of this ratio when the user resizes it.

var minSize: NSSize

The minimum size to which the window’s frame (including its title bar) can be sized.

var maxSize: NSSize

The maximum size to which the window’s frame (including its title bar) can be sized.

var isZoomed: Bool

A Boolean value that indicates whether the window is in a zoomed state.

func performZoom(Any?)

This action method simulates the user clicking the zoom box by momentarily highlighting the button and then zooming the window.

func zoom(Any?)

Toggles the size and location of the window between its standard state (which the application provides as the best size to display the window’s data) and its user state (a new size and location the user may have set by moving or resizing the window).

var resizeIncrements: NSSize

The window’s resizing increments.

