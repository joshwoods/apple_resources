

- Group Activities
- GroupSessionMessenger
- GroupSessionMessenger.Messages
-  GroupSessionMessenger.Messages.Iterator 

Structure

# GroupSessionMessenger.Messages.Iterator

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
struct Iterator
```

## Topics

### Instance Methods

func next() async -> GroupSessionMessenger.Messages&lt;Message>.Element?

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

func makeAsyncIterator() -> GroupSessionMessenger.Messages&lt;Message>.Iterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

typealias Element

The type of element produced by this asynchronous sequence.

