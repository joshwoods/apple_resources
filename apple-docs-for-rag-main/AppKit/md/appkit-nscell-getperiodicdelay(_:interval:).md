

- AppKit
- NSCell
-  getPeriodicDelay(\_:interval:) 

Instance Method

# getPeriodicDelay(\_:interval:)

Returns the initial delay and repeat values for continuous sending of action messages to target objects.

macOS

``` source
@MainActor
func getPeriodicDelay(
    _ delay: UnsafeMutablePointer,
    interval: UnsafeMutablePointer
)
```

## Parameters 

`delay`  

On input, a pointer to a floating-point variable. On output, the variable contains the current delay (measured in seconds) before messages are sent. This parameter must not be `NULL`.

`interval`  

On input, a pointer to a floating point variable. On output, the variable contains the interval (measured in seconds) at which messages are sent. This parameter must not be `NULL`.

## Discussion

The default implementation returns a delay of `0.2` and an interval of `0.025` seconds. Subclasses can override this method to supply their own delay and interval values.

## See Also

### Related Documentation

var isContinuous: Bool

A Boolean value indicating whether the cell sends its action message continuously during mouse tracking.

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

class var prefersTrackingUntilMouseUp: Bool

Returns a Boolean value that indicates whether tracking stops when the cursor leaves the cell.

