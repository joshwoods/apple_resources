

- AppKit
- NSCell
-  startTracking(at:in:) 

Instance Method

# startTracking(at:in:)

Begins tracking mouse events within the receiver.

macOS

``` source
@MainActor
func startTracking(
    at startPoint: NSPoint,
    in controlView: NSView
) -> Bool
```

## Parameters 

`startPoint`  

The initial location of the cursor.

`controlView`  

The `NSControl` object managing the receiver.

## Return Value

true if the receiver is set to respond continuously or set to respond when the mouse is dragged, otherwise false.

## Discussion

The `NSCell` implementation of trackMouse(with:in:of:untilMouseUp:) invokes this method when tracking begins. Subclasses can override this method to implement special mouse-tracking behavior at the beginning of mouse tracking—for example, displaying a special cursor.

## See Also

### Tracking the Mouse

func trackMouse(with: NSEvent, in: NSRect, of: NSView, untilMouseUp: Bool) -> Bool

Initiates the mouse tracking behavior in a cell.

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

