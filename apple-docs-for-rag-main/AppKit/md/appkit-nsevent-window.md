

- AppKit
- NSEvent
-  window 

Instance Property

# window

The window object associated with the event.

macOS

``` source
weak var window: NSWindow? { get }
```

## Discussion

Periodic events do not have a window. The result of accessing this property on a periodic event is undefined.

## See Also

### Getting general event information

var locationInWindow: NSPoint

The event location in the base coordinate system of the associated window.

var timestamp: TimeInterval

The time when the event occurred in seconds since system startup.

var windowNumber: Int

The identifier for the window device associated with the event.

var eventRef: UnsafeRawPointer?

An opaque Carbon type associated with this event.

var cgEvent: CGEvent?

The Core Graphics event object corresponding to this event.

class let foreverDuration: TimeInterval

The longest time duration possible.

