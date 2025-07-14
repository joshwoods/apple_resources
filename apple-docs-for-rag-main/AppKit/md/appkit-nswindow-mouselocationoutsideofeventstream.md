

- AppKit
- NSWindow
-  mouseLocationOutsideOfEventStream 

Instance Property

# mouseLocationOutsideOfEventStream

The current location of the pointer reckoned in the window’s base coordinate system, regardless of the current event being handled or of any events pending.

macOS

``` source
@MainActor
var mouseLocationOutsideOfEventStream: NSPoint { get }
```

## Discussion

For the same information in screen coordinates, use `NSEvent`’s mouseLocation.

## See Also

### Related Documentation

var currentEvent: NSEvent?

The last event object that the app retrieved from the event queue.

### Handling Mouse Events

var acceptsMouseMovedEvents: Bool

A Boolean value that indicates whether the window accepts mouse-moved events.

var ignoresMouseEvents: Bool

A Boolean value that indicates whether the window is transparent to mouse events.

class func windowNumber(at: NSPoint, belowWindowWithWindowNumber: Int) -> Int

Returns the number of the frontmost window that would be hit by a mouse-down at the specified screen location.

func trackEvents(matching: NSEvent.EventTypeMask, timeout: TimeInterval, mode: RunLoop.Mode, handler: (NSEvent?, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Tracks events that match the specified mask using the specified tracking handler until the tracking handler explicitly terminates tracking.

func performDrag(with: NSEvent)

Starts a window drag based on the specified mouse-down event.

class let foreverDuration: TimeInterval

The longest time duration possible.

