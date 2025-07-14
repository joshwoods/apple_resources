

- AppKit
- NSEvent
-  mouseLocation 

Type Property

# mouseLocation

Reports the current mouse position in screen coordinates.

macOS

``` source
class var mouseLocation: NSPoint { get }
```

## Return Value

The current mouse location in screen coordinates.

## Discussion

This method is similar to the mouseLocationOutsideOfEventStream method of NSWindow. It returns the location regardless of the current event or pending events. The difference between these methods is that mouseLocationOutsideOfEventStream returns a point in the receiving window’s coordinates, and mouseLocation returns the same information in screen coordinates.

## See Also

### Getting mouse event information

class var pressedMouseButtons: Int

The indices of the currently pressed mouse buttons.

class var doubleClickInterval: TimeInterval

The maximum number of seconds in which a second mouse click must occur for an event to be a double-click event.

var buttonNumber: Int

The button number for a mouse event.

var clickCount: Int

The number of mouse clicks associated with a mouse-down or mouse-up event.

var associatedEventsMask: NSEvent.EventTypeMask

The associated events mask of a mouse event.

