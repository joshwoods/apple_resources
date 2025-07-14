

- AppKit
- NSEvent
-  buttonNumber 

Instance Property

# buttonNumber

The button number for a mouse event.

macOS

``` source
var buttonNumber: Int { get }
```

## Discussion

This property is intended for use with the `NSOtherMouseDown`, `NSOtherMouseUp`, and `NSOtherMouseDragged` events, but will return values for `NSLeftMouse...` and `NSRightMouse...` events also. If this event is not a mouse event, the property is set to `0`.

## See Also

### Getting mouse event information

class var pressedMouseButtons: Int

The indices of the currently pressed mouse buttons.

class var doubleClickInterval: TimeInterval

The maximum number of seconds in which a second mouse click must occur for an event to be a double-click event.

class var mouseLocation: NSPoint

Reports the current mouse position in screen coordinates.

var clickCount: Int

The number of mouse clicks associated with a mouse-down or mouse-up event.

var associatedEventsMask: NSEvent.EventTypeMask

The associated events mask of a mouse event.

