

- AppKit
- NSWindow
-  zoom(\_:) 

Instance Method

# zoom(\_:)

Toggles the size and location of the window between its standard state (which the application provides as the best size to display the window’s data) and its user state (a new size and location the user may have set by moving or resizing the window).

macOS

``` source
@MainActor
func zoom(_ sender: Any?)
```

## Parameters 

`sender`  

The object sending the message.

## Discussion

For more information on the standard and user states, see windowWillUseStandardFrame(_:defaultFrame:).

Typically, the system invokes the zoom(_:) method after a user clicks the window’s zoom box, and performZoom(_:) may also invoke zoom(_:) programmatically. It performs the following steps:

1.  Invokes the windowWillUseStandardFrame(_:defaultFrame:) method, if the delegate or the window class implements it, to obtain a “best fit” frame for the window. If neither the delegate nor the window class implements the method, zoom(_:) uses a default frame. The default frame nearly fills the current screen that contains the largest part of the window’s current frame.

2.  Adjusts the resulting frame, if necessary, to fit on the current screen.

3.  Compares the resulting frame to the current frame to determine whether the window’s standard frame is currently displayed. If the current frame is within a few pixels of the standard frame in size and location, the system considers it a match.

4.  Determines a new frame. If the window is currently in the standard state, the new frame represents the user state, saved during a previous zoom. If the window is currently in the user state, the new frame represents the standard state, computed in step 1 above. If there’s no saved user state because there has been no previous zoom, the size and location of the window don’t change.

5.  Determines whether the window currently allows zooming. By default, zooming is allowed. If the window’s delegate implements the windowShouldZoom(_:toFrame:) method, zoom(_:) invokes that method. If the delegate doesn’t implement the method but the window does, zoom(_:) invokes the window’s version. windowShouldZoom(_:toFrame:) returns false if zooming isn’t currently allowed.

6.  If the window currently allows zooming, sets the new frame.

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

var resizeFlags: NSEvent.ModifierFlags

The flags field of the event record for the mouse-down event that initiated the resizing session.

var resizeIncrements: NSSize

The window’s resizing increments.

