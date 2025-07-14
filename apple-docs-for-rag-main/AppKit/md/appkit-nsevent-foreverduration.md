

- AppKit
- NSEvent
-  foreverDuration 

Type Property

# foreverDuration

The longest time duration possible.

macOS

``` source
class let foreverDuration: TimeInterval
```

## See Also

### Getting general event information

var locationInWindow: NSPoint

The event location in the base coordinate system of the associated window.

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

