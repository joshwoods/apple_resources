

- AppKit
- NSEvent
-  userData 

Instance Property

# userData

The data associated with a mouse-tracking event.

macOS

``` source
var userData: UnsafeMutableRawPointer? { get }
```

## Discussion

When you call addTrackingRect(_:owner:userData:assumeInside:) to set up a tracking rectangle, you can provide custom data to store in the event. AppKit makes that custom data available to you from this property.

This property is only valid when the event is of type NSMouseEntered or NSMouseExited. If you access this property for any other type of event, AppKit raises internalInconsistencyException.

## See Also

### Related Documentation

class func enterExitEvent(with: NSEvent.EventType, location: NSPoint, modifierFlags: NSEvent.ModifierFlags, timestamp: TimeInterval, windowNumber: Int, context: NSGraphicsContext?, eventNumber: Int, trackingNumber: Int, userData: UnsafeMutableRawPointer?) -> NSEvent?

Creates and returns a new event object that describes a tracking-rectangle or cursor-update event.

### Getting tracking area information

var eventNumber: Int

The counter value of the latest mouse or tracking-rectangle event object.

var trackingNumber: Int

The identifier of a mouse-tracking event.

var trackingArea: NSTrackingArea?

The tracking area for the event.

