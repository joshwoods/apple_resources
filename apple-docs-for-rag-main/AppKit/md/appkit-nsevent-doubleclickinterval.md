

- AppKit
- NSEvent
-  doubleClickInterval 

Type Property

# doubleClickInterval

The maximum number of seconds in which a second mouse click must occur for an event to be a double-click event.

macOS 10.6+

``` source
class var doubleClickInterval: TimeInterval { get }
```

## Return Value

The double-click time interval, in seconds.

## Discussion

This is a system setting. You can’t change the value by overriding this method.

## See Also

### Getting mouse event information

class var pressedMouseButtons: Int

The indices of the currently pressed mouse buttons.

class var mouseLocation: NSPoint

Reports the current mouse position in screen coordinates.

var buttonNumber: Int

The button number for a mouse event.

var clickCount: Int

The number of mouse clicks associated with a mouse-down or mouse-up event.

var associatedEventsMask: NSEvent.EventTypeMask

The associated events mask of a mouse event.

