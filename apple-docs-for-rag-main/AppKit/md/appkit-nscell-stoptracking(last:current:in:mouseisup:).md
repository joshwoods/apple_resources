

- AppKit
- NSCell
-  stopTracking(last:current:in:mouseIsUp:) 

Instance Method

# stopTracking(last:current:in:mouseIsUp:)

Stops tracking mouse events within the receiver.

macOS

``` source
@MainActor
func stopTracking(
    last lastPoint: NSPoint,
    current stopPoint: NSPoint,
    in controlView: NSView,
    mouseIsUp flag: Bool
)
```

## Parameters 

`lastPoint`  

Contains the previous position of the cursor.

`stopPoint`  

The current location of the cursor.

`controlView`  

The `NSControl` object managing the receiver.

`flag`  

If true, this method was invoked because the user released the mouse button; otherwise, if false, the cursor left the designated tracking rectangle.

## Discussion

The default `NSCell` implementation of trackMouse(with:in:of:untilMouseUp:) invokes this method when the cursor has left the bounds of the receiver or the mouse button goes up. The default `NSCell` implementation of this method does nothing. Subclasses often override this method to provide customized tracking behavior. The following example increments the state of a tristate cell when the mouse button is clicked:

```
- (void)stopTracking:(NSPoint)lastPoint at:(NSPoint)stopPoint
    inView:(NSView *)controlView mouseIsUp:(BOOL)flag
{
    if (flag == YES) {
        [self setTriState:([self triState]+1)];
    }
}
```

## See Also

### Tracking the Mouse

func trackMouse(with: NSEvent, in: NSRect, of: NSView, untilMouseUp: Bool) -> Bool

Initiates the mouse tracking behavior in a cell.

func startTracking(at: NSPoint, in: NSView) -> Bool

Begins tracking mouse events within the receiver.

func continueTracking(last: NSPoint, current: NSPoint, in: NSView) -> Bool

Returns a Boolean value that indicates whether mouse tracking should continue in the receiving cell.

var mouseDownFlags: Int

The modifier flags for the last (left) mouse-down event.

class var prefersTrackingUntilMouseUp: Bool

Returns a Boolean value that indicates whether tracking stops when the cursor leaves the cell.

func getPeriodicDelay(UnsafeMutablePointer&lt;Float>, interval: UnsafeMutablePointer&lt;Float>)

Returns the initial delay and repeat values for continuous sending of action messages to target objects.

