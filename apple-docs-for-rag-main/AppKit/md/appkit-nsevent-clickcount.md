

- AppKit
- NSEvent
-  clickCount 

Instance Property

# clickCount

The number of mouse clicks associated with a mouse-down or mouse-up event.

macOS

``` source
var clickCount: Int { get }
```

## Discussion

Raises an `NSInternalInconsistencyException` if accessed on a non-mouse event.

This property is set to `0` for a mouse-up event if a time threshold has passed since the corresponding mouse-down event. This is because if this time threshold passes before the mouse button is released, it is no longer considered a mouse click, but a mouse-down event followed by a mouse-up event.

The return value of this method is meaningless for events other than mouse-down or mouse-up events.

## See Also

### Related Documentation

class func mouseEvent(with: NSEvent.EventType, location: NSPoint, modifierFlags: NSEvent.ModifierFlags, timestamp: TimeInterval, windowNumber: Int, context: NSGraphicsContext?, eventNumber: Int, clickCount: Int, pressure: Float) -> NSEvent?

Creates and returns a new event object that describes a mouse-down, -up, -moved, or -dragged event.

### Getting mouse event information

class var pressedMouseButtons: Int

The indices of the currently pressed mouse buttons.

class var doubleClickInterval: TimeInterval

The maximum number of seconds in which a second mouse click must occur for an event to be a double-click event.

class var mouseLocation: NSPoint

Reports the current mouse position in screen coordinates.

var buttonNumber: Int

The button number for a mouse event.

var associatedEventsMask: NSEvent.EventTypeMask

The associated events mask of a mouse event.

