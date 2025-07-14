

- ARKit
- ARKitSession
- ARKitSession.Events
-  ARKitSession.Events.Iterator 

Structure

# ARKitSession.Events.Iterator

A type that provides a sequence’s iteration interface and encapsulates its iteration state.

visionOS 1.0+

``` source
struct Iterator
```

## Topics

### Type aliases

typealias Element

A type representing a sequence’s elements.

### Instance methods

func next() async -> ARKitSession.Events.Element?

Returns the next element in a sequence.

## Relationships

### Conforms To

- AsyncIteratorProtocol

