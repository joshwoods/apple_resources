

- AppKit
- NSEvent
-  windowNumber 

Instance Property

# windowNumber

The identifier for the window device associated with the event.

macOS

``` source
var windowNumber: Int { get }
```

## Discussion

Periodic events do not have a window. The result of accessing this property on a periodic event is undefined.

## See Also

### Getting general event information

var locationInWindow: NSPoint

The event location in the base coordinate system of the associated window.

var timestamp: TimeInterval

The time when the event occurred in seconds since system startup.

var window: NSWindow?

The window object associated with the event.

var eventRef: UnsafeRawPointer?

An opaque Carbon type associated with this event.

var cgEvent: CGEvent?

The Core Graphics event object corresponding to this event.

class let foreverDuration: TimeInterval

The longest time duration possible.

