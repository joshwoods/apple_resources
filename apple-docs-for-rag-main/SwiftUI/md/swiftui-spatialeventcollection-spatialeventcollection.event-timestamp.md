

- SwiftUI
- SpatialEventCollection
- SpatialEventCollection.Event
-  timestamp 

Instance Property

# timestamp

The time the event was processed.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+watchOS 11.0+

``` source
var timestamp: TimeInterval
```

## See Also

### Identifying the event

var id: SpatialEventCollection.Event.ID

An identifier that uniquely identifies the event over its lifetime.

struct ID

A value that uniquely identifies an event over the course of its lifetime.

var kind: SpatialEventCollection.Event.Kind

The event’s input source.

enum Kind

The possible input sources or modes of an event.

var modifierKeys: EventModifiers

The set of active modifier keys at the time of this event.

