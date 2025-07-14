

- SwiftUI
- SpatialEventCollection
- SpatialEventCollection.Event
-  SpatialEventCollection.Event.Kind 

Enumeration

# SpatialEventCollection.Event.Kind

The possible input sources or modes of an event.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+watchOS 11.0+

``` source
enum Kind
```

## Topics

### Getting the event type

case directPinch

An event generated from a pinching hand in close proximity to content.

case indirectPinch

An event generated from an indirectly targeted pinching hand.

case pointer

An event representing a click-based, indirect input device describing the input sequence from click to click release.

case touch

An event generated from a touch directly targeting content.

### Enumeration Cases

case pencil

An event generated from a pencil making contact with content.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Identifying the event

var timestamp: TimeInterval

The time the event was processed.

var id: SpatialEventCollection.Event.ID

An identifier that uniquely identifies the event over its lifetime.

struct ID

A value that uniquely identifies an event over the course of its lifetime.

var kind: SpatialEventCollection.Event.Kind

The event’s input source.

var modifierKeys: EventModifiers

The set of active modifier keys at the time of this event.

