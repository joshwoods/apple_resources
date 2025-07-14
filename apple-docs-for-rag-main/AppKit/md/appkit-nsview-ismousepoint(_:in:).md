

- AppKit
- NSView
-  isMousePoint(\_:in:) 

Instance Method

# isMousePoint(\_:in:)

Returns whether a region of the view contains a specified point, accounting for whether the view is flipped or not.

macOS

``` source
@MainActor
func isMousePoint(
    _ point: NSPoint,
    in rect: NSRect
) -> Bool
```

## Parameters 

`point`  

A point that is expressed in the view’s coordinate system. This point generally represents the hot spot of the mouse cursor.

`rect`  

A rectangle that is expressed in the view’s coordinate system.

## Return Value

true if `aRect` contains `aPoint`, false otherwise.

## Discussion

Point-in-rectangle functions generally assume that the bottom edge of a rectangle is outside of the rectangle boundaries, while the upper edge is inside the boundaries. This method views `aRect` from the point of view of the user—that is, this method always treats the bottom edge of the rectangle as the one closest to the bottom edge of the user’s screen. By making this adjustment, this function ensures consistent mouse-detection behavior from the user’s perspective.

Never use the Foundation’s NSPointInRect(_:_:) function as a substitute for this method. It doesn’t account for flipped coordinate systems.

## See Also

### Related Documentation

func convert(NSPoint, from: NSView?) -> NSPoint

Converts a point from the coordinate system of a given view to that of the view.

func NSMouseInRect(NSPoint, NSRect, Bool) -> Bool

Returns a Boolean value that indicates whether the point is in the specified rectangle.

var isFlipped: Bool

A Boolean value indicating whether the view uses a flipped coordinate system.

### Handling Events in the View

func acceptsFirstMouse(for: NSEvent?) -> Bool

Overridden by subclasses to return true if the view should be sent a mouseDown(with:) message for an initial mouse-down event, false if not.

func hitTest(NSPoint) -> NSView?

Returns the farthest descendant of the view in the view hierarchy (including itself) that contains a specified point, or `nil` if that point lies completely outside the view.

func performKeyEquivalent(with: NSEvent) -> Bool

Implemented by subclasses to respond to key equivalents (also known as keyboard shortcuts).

func rightMouseDown(with: NSEvent)

Informs the receiver that the user has pressed the right mouse button.

var mouseDownCanMoveWindow: Bool

A Boolean value indicating whether the view can pass mouse down events through to its superviews.

var inputContext: NSTextInputContext?

The text input context object for the view.

