

- Shared With You
-  SWHighlightPersistenceEventTrigger 

Enumeration

# SWHighlightPersistenceEventTrigger

Signifies the type of persistence event trigger.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
enum SWHighlightPersistenceEventTrigger
```

## Topics

### Persistence actions

case created

Signifies a creation event.

case deleted

Signifies a deletion event.

case renamed

Signifies a rename event.

case moved

Signifies a move event.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Accessing an event trigger

var persistenceEventTrigger: SWHighlightPersistenceEventTrigger

The persistence event trigger for the highlight.

