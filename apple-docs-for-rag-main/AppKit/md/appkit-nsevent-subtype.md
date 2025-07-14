

- AppKit
- NSEvent
-  subtype 

Instance Property

# subtype

The event’s subtype.

macOS

``` source
var subtype: NSEvent.EventSubtype { get }
```

## Discussion

Access this property only if the event is a mouse event or if the type property contains NSAppKitDefined, NSSystemDefined, NSApplicationDefined, or NSPeriodic. If you access this property for other types, AppKit raises internalInconsistencyException. For information about predefined mouse and tablet subtypes, see `Getting Unicode Values`.

NSPeriodic events don’t use this property.

## See Also

### Related Documentation

var data1: Int

Additional data associated with this event.

var data2: Int

Additional data associated with this event.

class func otherEvent(with: NSEvent.EventType, location: NSPoint, modifierFlags: NSEvent.ModifierFlags, timestamp: TimeInterval, windowNumber: Int, context: NSGraphicsContext?, subtype: Int16, data1: Int, data2: Int) -> NSEvent?

Creates and returns a new event object that describes a custom event.

### Getting the event type

var type: NSEvent.EventType

The event’s type.

enum EventType

Constants for the types of events that responder objects can handle.

struct EventTypeMask

Constants that you use to filter out specific event types from the stream of incoming events.

enum EventSubtype

Subtypes for various types of events.

