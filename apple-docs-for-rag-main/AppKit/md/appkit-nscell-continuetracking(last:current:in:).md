

- AppKit
- NSCell
-  continueTracking(last:current:in:) 

Instance Method

# continueTracking(last:current:in:)

Returns a Boolean value that indicates whether mouse tracking should continue in the receiving cell.

macOS

``` source
@MainActor
func continueTracking(
    last lastPoint: NSPoint,
    current currentPoint: NSPoint,
    in controlView: NSView
) -> Bool
```

## Parameters 

`lastPoint`  

Contains either the initial location of the cursor when tracking began or the previous current point.

`currentPoint`  

The current location of the cursor.

`controlView`  

The `NSControl` object managing the receiver.

## Return Value

true if mouse tracking should continue, otherwise false.

## Discussion

This method is invoked in trackMouse(with:in:of:untilMouseUp:). The default implementation returns true if the cell is set to continuously send action messages to its target when the mouse button is down or the mouse is being dragged. Subclasses can override this method to provide more sophisticated tracking behavior.

## See Also

### Tracking the Mouse

func trackMouse(with: NSEvent, in: NSRect, of: NSView, untilMouseUp: Bool) -> Bool

Initiates the mouse tracking behavior in a cell.

func startTracking(at: NSPoint, in: NSView) -> Bool

Begins tracking mouse events within the receiver.

func stopTracking(last: NSPoint, current: NSPoint, in: NSView, mouseIsUp: Bool)

Stops tracking mouse events within the receiver.

var mouseDownFlags: Int

The modifier flags for the last (left) mouse-down event.

class var prefersTrackingUntilMouseUp: Bool

Returns a Boolean value that indicates whether tracking stops when the cursor leaves the cell.

func getPeriodicDelay(UnsafeMutablePointer&lt;Float>, interval: UnsafeMutablePointer&lt;Float>)

Returns the initial delay and repeat values for continuous sending of action messages to target objects.

