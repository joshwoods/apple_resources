

- Group Activities
- SystemCoordinator
-  SystemCoordinator.ParticipantStates 

Structure

# SystemCoordinator.ParticipantStates

An asynchronous sequence that reports the current person’s ability to participate in a shared context.

visionOS 1.0+

``` source
struct ParticipantStates
```

## Topics

### Creating an iterator

func makeAsyncIterator() -> SystemCoordinator.ParticipantStates.Iterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

struct Iterator

typealias Element

The type of element produced by this asynchronous sequence.

### Type Aliases

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

### Default Implementations

AsyncSequence Implementations

## Relationships

### Conforms To

- AsyncSequence
- Sendable

## See Also

### Getting the participant state

var localParticipantState: SystemCoordinator.ParticipantState

The current participant’s level of support for an activity that takes place in a shared simulation space.

var localParticipantStates: SystemCoordinator.ParticipantStates

An asynchronous sequence that reports changes to the local participant’s state.

