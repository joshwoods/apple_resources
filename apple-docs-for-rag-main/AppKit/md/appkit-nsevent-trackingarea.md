

- AppKit
- NSEvent
-  trackingArea 

Instance Property

# trackingArea

The tracking area for the event.

macOS 10.5+

``` source
var trackingArea: NSTrackingArea? { get }
```

## Discussion

If you access this property on an event object that is not a mouse-tracking event — that is, its event type isn’t NSMouseEntered, NSMouseExited, or NSCursorUpdate —AppKit raises an internalInconsistencyException.

If the event corresponds to a tracking rectangle installed with the addTrackingRect(_:owner:userData:assumeInside:) method of NSView, the value of this property is `nil`. The trackingNumber property contains either an NSTrackingArea object or NSView.TrackingRectTag, depending on how AppKit generated the event.

## See Also

### Getting tracking area information

var eventNumber: Int

The counter value of the latest mouse or tracking-rectangle event object.

var trackingNumber: Int

The identifier of a mouse-tracking event.

var userData: UnsafeMutableRawPointer?

The data associated with a mouse-tracking event.

