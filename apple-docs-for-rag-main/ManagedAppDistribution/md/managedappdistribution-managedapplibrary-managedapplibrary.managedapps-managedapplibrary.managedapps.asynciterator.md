

- ManagedAppDistribution
- ManagedAppLibrary
- ManagedAppLibrary.ManagedApps
-  ManagedAppLibrary.ManagedApps.AsyncIterator 

Structure

# ManagedAppLibrary.ManagedApps.AsyncIterator

The iterator for managed apps.

iOS 17.2+iPadOS 17.2+visionOS 2.4+

``` source
struct AsyncIterator
```

## Topics

### Iterating

typealias Element

The type of element this asynchronous sequence produces.

func next() async throws -> ManagedAppLibrary.ManagedApps.AsyncIterator.Element?

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

### Instance Methods

func next(isolation: isolated (any Actor)?) async throws(ManagedAppLibrary.ManagedApps.AsyncIterator.Failure) -> ManagedAppLibrary.ManagedApps.AsyncIterator.Element?

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

### Type Aliases

typealias Failure

The type of failure produced by iteration.

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol

## See Also

### Obtaining managed apps

typealias Element

The type of element this asynchronous sequence produces.

func makeAsyncIterator() -> ManagedAppLibrary.ManagedApps.AsyncIterator

Creates the asynchronous iterator that produces results from this asynchronous sequence.

