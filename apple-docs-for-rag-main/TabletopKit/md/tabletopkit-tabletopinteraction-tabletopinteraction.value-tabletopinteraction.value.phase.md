

- TabletopKit
- TabletopInteraction
- TabletopInteraction.Value
-  TabletopInteraction.Value.Phase 

Enumeration

# TabletopInteraction.Value.Phase

The stages of players interacting with equipment on the table.

visionOS 2.0+

``` source
enum Phase
```

## Topics

### Enumeration Cases

case cancelled

case ended

case started

case update

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Getting the phases

var gesturePhase: TabletopInteraction.Value.Phase?

the current phase of the gesture

Deprecated

var phase: TabletopInteraction.Value.Phase

the current phase of the overall interaction

