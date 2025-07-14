

- SwiftUI
- SpatialEventCollection
- SpatialEventCollection.Event
-  SpatialEventCollection.Event.Phase 

Enumeration

# SpatialEventCollection.Event.Phase

The states that an event can have.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+watchOS 11.0+

``` source
enum Phase
```

## Topics

### Getting the phase

case active

The phase is active and the state associated with it is guaranteed to produce at least one more update.

case cancelled

The state associated with this phase was canceled and won’t produce any more updates.

case ended

The state associated with this phase ended normally and won’t produce any more updates.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Getting the event’s current phase

var phase: SpatialEventCollection.Event.Phase

The phase of the event.

