

- AppKit
- NSWindow
-  acceptsMouseMovedEvents 

Instance Property

# acceptsMouseMovedEvents

A Boolean value that indicates whether the window accepts mouse-moved events.

macOS

``` source
@MainActor
var acceptsMouseMovedEvents: Bool { get set }
```

## Discussion

The value of this property is true when the window accepts (and distributes) mouse-moved events; otherwise, false. By default the value is false.

## See Also

### Handling Mouse Events

var ignoresMouseEvents: Bool

A Boolean value that indicates whether the window is transparent to mouse events.

var mouseLocationOutsideOfEventStream: NSPoint

The current location of the pointer reckoned in the window’s base coordinate system, regardless of the current event being handled or of any events pending.

class func windowNumber(at: NSPoint, belowWindowWithWindowNumber: Int) -> Int

Returns the number of the frontmost window that would be hit by a mouse-down at the specified screen location.

func trackEvents(matching: NSEvent.EventTypeMask, timeout: TimeInterval, mode: RunLoop.Mode, handler: (NSEvent?, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Tracks events that match the specified mask using the specified tracking handler until the tracking handler explicitly terminates tracking.

func performDrag(with: NSEvent)

Starts a window drag based on the specified mouse-down event.

class let foreverDuration: TimeInterval

The longest time duration possible.

