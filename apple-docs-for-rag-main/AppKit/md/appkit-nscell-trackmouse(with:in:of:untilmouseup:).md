

- AppKit
- NSCell
-  trackMouse(with:in:of:untilMouseUp:) 

Instance Method

# trackMouse(with:in:of:untilMouseUp:)

Initiates the mouse tracking behavior in a cell.

macOS

``` source
@MainActor
func trackMouse(
    with event: NSEvent,
    in cellFrame: NSRect,
    of controlView: NSView,
    untilMouseUp flag: Bool
) -> Bool
```

## Parameters 

`event`  

The event that caused the mouse tracking to occur.

`cellFrame`  

The receiver’s frame rectangle.

`controlView`  

The view containing the receiver. This is usually an `NSControl` object.

`flag`  

If true, mouse tracking continues until the user releases the mouse button. If false, tracking continues until the cursor leaves the tracking rectangle, specified by the `cellFrame` parameter, regardless of the mouse button state. See the discussion for more information.

## Return Value

true if the mouse tracking conditions are met, otherwise false.

## Discussion

This method is generally not overridden because the default implementation invokes other `NSCell` methods that can be overridden to handle specific events in a dragging session. This method’s return value depends on the `untilMouseUp` flag. If `untilMouseUp` is set to true, this method returns true if the mouse button goes up while the cursor is anywhere; false, otherwise. If `untilMouseUp` is set to false, this method returns true if the mouse button goes up while the cursor is within `cellFrame`; false, otherwise.

This method first invokes startTracking(at:in:). If that method returns true, then as mouse-dragged events are intercepted, continueTracking(last:current:in:) is invoked until either the method returns false or the mouse is released. Finally, stopTracking(last:current:in:mouseIsUp:) is invoked if the mouse is released. If `untilMouseUp` is true, it’s invoked when the mouse button goes up while the cursor is anywhere. If `untilMouseUp` is false, it’s invoked when the mouse button goes up while the cursor is within `cellFrame`. You usually override one or more of these methods to respond to specific mouse events.

## See Also

### Tracking the Mouse

func startTracking(at: NSPoint, in: NSView) -> Bool

Begins tracking mouse events within the receiver.

func continueTracking(last: NSPoint, current: NSPoint, in: NSView) -> Bool

Returns a Boolean value that indicates whether mouse tracking should continue in the receiving cell.

func stopTracking(last: NSPoint, current: NSPoint, in: NSView, mouseIsUp: Bool)

Stops tracking mouse events within the receiver.

var mouseDownFlags: Int

The modifier flags for the last (left) mouse-down event.

class var prefersTrackingUntilMouseUp: Bool

Returns a Boolean value that indicates whether tracking stops when the cursor leaves the cell.

func getPeriodicDelay(UnsafeMutablePointer&lt;Float>, interval: UnsafeMutablePointer&lt;Float>)

Returns the initial delay and repeat values for continuous sending of action messages to target objects.

