

- AppKit
- NSEvent
-  data2 

Instance Property

# data2

Additional data associated with this event.

macOS

``` source
var data2: Int { get }
```

## Discussion

The originator of the event defines the data in this property, and the data is dependent on the event type. If the type of this event isn’t NSAppKitDefined, NSSystemDefined, NSApplicationDefined, or NSPeriodic, accessing this property raises internalInconsistencyException.

NSPeriodic events don’t use this property.

## See Also

### Related Documentation

var subtype: NSEvent.EventSubtype

The event’s subtype.

class func otherEvent(with: NSEvent.EventType, location: NSPoint, modifierFlags: NSEvent.ModifierFlags, timestamp: TimeInterval, windowNumber: Int, context: NSGraphicsContext?, subtype: Int16, data1: Int, data2: Int) -> NSEvent?

Creates and returns a new event object that describes a custom event.

### Getting custom event information

var data1: Int

Additional data associated with this event.

