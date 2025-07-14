

- AppKit
- NSEvent
-  cgEvent 

Instance Property

# cgEvent

The Core Graphics event object corresponding to this event.

macOS 10.5+

``` source
var cgEvent: CGEvent? { get }
```

## Discussion

The CGEvent opaque type returned is autoreleased. If no `CGEventRef` object corresponding to the `NSEvent` object can be created, this method returns `NULL`.

## See Also

### Related Documentation

init?(cgEvent: CGEvent)

Creates and returns an event object for a Core Graphics event.

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

class let foreverDuration: TimeInterval

The longest time duration possible.

