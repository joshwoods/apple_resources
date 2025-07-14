

- AppKit
- NSEvent
-  locationInWindow 

Instance Property

# locationInWindow

The event location in the base coordinate system of the associated window.

macOS

``` source
var locationInWindow: NSPoint { get }
```

## Discussion

This property applies to mouse events. For non-mouse events the value of this property is undefined.

With NSMouseMoved and possibly other events, the event can have a `nil` window (that is, the window property contains nil). In this case, this property contains the event location in screen coordinates.

In a method of a custom view that handles mouse events, you commonly use this property with the convert(_:from:) method of NSView to get the mouse location in the view’s coordinate system. The following code shows how to perform this conversion. The y coordinate in the returned point starts from a base of 1, and not 0.

```
NSPoint event_location = theEvent.locationInWindow;
NSPoint local_point = [self convertPoint:event_location fromView:nil];
```

## See Also

### Getting general event information

var timestamp: TimeInterval

The time when the event occurred in seconds since system startup.

var window: NSWindow?

The window object associated with the event.

var windowNumber: Int

The identifier for the window device associated with the event.

var eventRef: UnsafeRawPointer?

An opaque Carbon type associated with this event.

var cgEvent: CGEvent?

The Core Graphics event object corresponding to this event.

class let foreverDuration: TimeInterval

The longest time duration possible.

