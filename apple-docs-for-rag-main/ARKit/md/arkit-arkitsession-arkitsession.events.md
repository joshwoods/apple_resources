

- ARKit
- ARKitSession
-  ARKitSession.Events 

Structure

# ARKitSession.Events

A sequence of events.

visionOS 1.0+

``` source
struct Events
```

## Topics

### Structures

struct Iterator

A type that provides a sequence’s iteration interface and encapsulates its iteration state.

### Instance Methods

func makeAsyncIterator() -> ARKitSession.Events.Iterator

### Type Aliases

typealias Element

A type representing a sequence’s elements.

## Relationships

### Conforms To

- AsyncSequence

## See Also

### Observing a session

var events: ARKitSession.Events

An asynchronous sequence of events that provide updates to the current authorization status of the session.

enum Event

The kinds of events that can occur in a session.

var description: String

A textual representation of this session.

