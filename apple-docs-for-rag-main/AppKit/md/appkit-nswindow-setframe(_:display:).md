

- AppKit
- NSWindow
-  setFrame(\_:display:) 

Instance Method

# setFrame(\_:display:)

Sets the origin and size of the window’s frame rectangle according to a given frame rectangle, thereby setting its position and size onscreen.

macOS

``` source
@MainActor
func setFrame(
    _ frameRect: NSRect,
    display flag: Bool
)
```

## Parameters 

`frameRect`  

The frame rectangle for the window, including the title bar.

`flag`  

Specifies whether the window redraws the views that need to be displayed. When true the window sends a displayIfNeeded() message down its view hierarchy, thus redrawing all views.

## Discussion

Note that the window server limits window position coordinates to ±16,000 and sizes to 10,000.

## See Also

### Related Documentation

func setFrame(from: NSWindow.PersistableFrameDescriptor)

Sets the window’s frame rectangle from a given string representation.

class func frameRect(forContentRect: NSRect, styleMask: NSWindow.StyleMask) -> NSRect

Returns the frame rectangle used by a window with a given content rectangle and window style.

func setFrameUsingName(NSWindow.FrameAutosaveName) -> Bool

Sets the window’s frame rectangle by reading the rectangle data stored under a given name from the defaults system.

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

var resizeFlags: NSEvent.ModifierFlags

The flags field of the event record for the mouse-down event that initiated the resizing session.

var resizeIncrements: NSSize

The window’s resizing increments.

