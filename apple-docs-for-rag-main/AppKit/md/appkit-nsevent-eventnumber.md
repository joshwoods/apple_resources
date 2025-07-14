

- AppKit
- NSEvent
-  eventNumber 

Instance Property

# eventNumber

The counter value of the latest mouse or tracking-rectangle event object.

macOS

``` source
var eventNumber: Int { get }
```

## Discussion

Every system-generated mouse and tracking-rectangle event increments this counter. If you access this property on an event of an unsupported type, AppKit raises internalInconsistencyException.

## See Also

### Related Documentation

class func enterExitEvent(with: NSEvent.EventType, location: NSPoint, modifierFlags: NSEvent.ModifierFlags, timestamp: TimeInterval, windowNumber: Int, context: NSGraphicsContext?, eventNumber: Int, trackingNumber: Int, userData: UnsafeMutableRawPointer?) -> NSEvent?

Creates and returns a new event object that describes a tracking-rectangle or cursor-update event.

class func mouseEvent(with: NSEvent.EventType, location: NSPoint, modifierFlags: NSEvent.ModifierFlags, timestamp: TimeInterval, windowNumber: Int, context: NSGraphicsContext?, eventNumber: Int, clickCount: Int, pressure: Float) -> NSEvent?

Creates and returns a new event object that describes a mouse-down, -up, -moved, or -dragged event.

### Getting tracking area information

var trackingNumber: Int

The identifier of a mouse-tracking event.

var trackingArea: NSTrackingArea?

The tracking area for the event.

var userData: UnsafeMutableRawPointer?

The data associated with a mouse-tracking event.

