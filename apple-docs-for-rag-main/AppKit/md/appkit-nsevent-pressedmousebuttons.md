

- AppKit
- NSEvent
-  pressedMouseButtons 

Type Property

# pressedMouseButtons

The indices of the currently pressed mouse buttons.

macOS 10.6+

``` source
class var pressedMouseButtons: Int { get }
```

## Return Value

The indices of the currently depressed mouse buttons.

## Discussion

A return value of `1 =2` correspond to other mouse buttons.

This returns the state of devices combined with synthesized events at the moment, independent of which events have been delivered via the event stream, so this method is not suitable for tracking.

## See Also

### Getting mouse event information

class var doubleClickInterval: TimeInterval

The maximum number of seconds in which a second mouse click must occur for an event to be a double-click event.

class var mouseLocation: NSPoint

Reports the current mouse position in screen coordinates.

var buttonNumber: Int

The button number for a mouse event.

var clickCount: Int

The number of mouse clicks associated with a mouse-down or mouse-up event.

var associatedEventsMask: NSEvent.EventTypeMask

The associated events mask of a mouse event.

