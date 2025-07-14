

- Group Activities
- SystemCoordinator
- SystemCoordinator.ParticipantStates
-  SystemCoordinator.ParticipantStates.Iterator 

Structure

# SystemCoordinator.ParticipantStates.Iterator

visionOS 1.0+

``` source
struct Iterator
```

## Topics

### Instance Methods

func next() async -> SystemCoordinator.ParticipantStates.Element?

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

### Type Aliases

typealias Element

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol
- Sendable

## See Also

### Creating an iterator

func makeAsyncIterator() -> SystemCoordinator.ParticipantStates.Iterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

typealias Element

The type of element produced by this asynchronous sequence.

