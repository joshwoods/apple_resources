

- AppKit
- NSCell
-  mouseDownFlags 

Instance Property

# mouseDownFlags

The modifier flags for the last (left) mouse-down event.

macOS

``` source
@MainActor
var mouseDownFlags: Int { get }
```

## Discussion

The value of this property is the value of the modifier flags from the most recent NSEvent object representing a mouse-down event. If tracking has not yet occurred or the event contained no modifier keys, the value of this property is `0`.

## See Also

### Related Documentation

var modifierFlags: NSEvent.ModifierFlags

An integer bit field that indicates the pressed modifier keys.

### Tracking the Mouse

func trackMouse(with: NSEvent, in: NSRect, of: NSView, untilMouseUp: Bool) -> Bool

Initiates the mouse tracking behavior in a cell.

func startTracking(at: NSPoint, in: NSView) -> Bool

Begins tracking mouse events within the receiver.

func continueTracking(last: NSPoint, current: NSPoint, in: NSView) -> Bool

Returns a Boolean value that indicates whether mouse tracking should continue in the receiving cell.

func stopTracking(last: NSPoint, current: NSPoint, in: NSView, mouseIsUp: Bool)

Stops tracking mouse events within the receiver.

class var prefersTrackingUntilMouseUp: Bool

Returns a Boolean value that indicates whether tracking stops when the cursor leaves the cell.

func getPeriodicDelay(UnsafeMutablePointer&lt;Float>, interval: UnsafeMutablePointer&lt;Float>)

Returns the initial delay and repeat values for continuous sending of action messages to target objects.

