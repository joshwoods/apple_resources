

- Group Activities
- GroupSession
- GroupSession.Sessions
-  GroupSession.Sessions.Iterator 

Structure

# GroupSession.Sessions.Iterator

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
struct Iterator
```

## Topics

### Instance Methods

func next() async -> GroupSession&lt;ActivityType>?

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

func makeAsyncIterator() -> GroupSession&lt;ActivityType>.Sessions.Iterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

typealias Element

The type of element produced by this asynchronous sequence.

