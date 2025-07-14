

- AppKit
- NSCell
-  prefersTrackingUntilMouseUp 

Type Property

# prefersTrackingUntilMouseUp

Returns a Boolean value that indicates whether tracking stops when the cursor leaves the cell.

macOS

``` source
@MainActor
class var prefersTrackingUntilMouseUp: Bool { get }
```

## Return Value

true if tracking stops when the cursor leaves the cell, otherwise false.

## Discussion

The default implementation returns false. Subclasses may override this method to return a different value.

## See Also

### Tracking the Mouse

func trackMouse(with: NSEvent, in: NSRect, of: NSView, untilMouseUp: Bool) -> Bool

Initiates the mouse tracking behavior in a cell.

func startTracking(at: NSPoint, in: NSView) -> Bool

Begins tracking mouse events within the receiver.

func continueTracking(last: NSPoint, current: NSPoint, in: NSView) -> Bool

Returns a Boolean value that indicates whether mouse tracking should continue in the receiving cell.

func stopTracking(last: NSPoint, current: NSPoint, in: NSView, mouseIsUp: Bool)

Stops tracking mouse events within the receiver.

var mouseDownFlags: Int

The modifier flags for the last (left) mouse-down event.

func getPeriodicDelay(UnsafeMutablePointer&lt;Float>, interval: UnsafeMutablePointer&lt;Float>)

Returns the initial delay and repeat values for continuous sending of action messages to target objects.

