

- AppKit
- NSEvent
-  trackingNumber 

Instance Property

# trackingNumber

The identifier of a mouse-tracking event.

macOS

``` source
var trackingNumber: Int { get }
```

## Discussion

This property contains either an NSTrackingArea object or an NSView.TrackingRectTag constant, depending on how AppKit generated the event. Valid mouse-tracking event types are NSMouseEntered, NSMouseExited, and NSCursorUpdate. For other types of events, accessing this property raises internalInconsistencyException.

## See Also

### Related Documentation

class func enterExitEvent(with: NSEvent.EventType, location: NSPoint, modifierFlags: NSEvent.ModifierFlags, timestamp: TimeInterval, windowNumber: Int, context: NSGraphicsContext?, eventNumber: Int, trackingNumber: Int, userData: UnsafeMutableRawPointer?) -> NSEvent?

Creates and returns a new event object that describes a tracking-rectangle or cursor-update event.

func addTrackingRect(NSRect, owner: Any, userData: UnsafeMutableRawPointer?, assumeInside: Bool) -> NSView.TrackingRectTag

Establishes an area for tracking mouse-entered and mouse-exited events within the view and returns a tag that identifies the tracking rectangle.

### Getting tracking area information

var eventNumber: Int

The counter value of the latest mouse or tracking-rectangle event object.

var trackingArea: NSTrackingArea?

The tracking area for the event.

var userData: UnsafeMutableRawPointer?

The data associated with a mouse-tracking event.

