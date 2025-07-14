

- AppKit
- NSEvent
-  timestamp 

Instance Property

# timestamp

The time when the event occurred in seconds since system startup.

macOS

``` source
var timestamp: TimeInterval { get }
```

## See Also

### Related Documentation

var systemUptime: TimeInterval

The amount of time the system has been awake since the last time it was restarted.

### Getting general event information

var locationInWindow: NSPoint

The event location in the base coordinate system of the associated window.

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

