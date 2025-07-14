

- Group Activities
- GroupSessionJournal
- GroupSessionJournal.Attachments
-  GroupSessionJournal.Attachments.Iterator 

Structure

# GroupSessionJournal.Attachments.Iterator

The asynchronous iterator that produces a sequence of attachments.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct Iterator
```

## Topics

### Instance Methods

func next() async -> GroupSessionJournal.Attachments.Element?

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

func makeAsyncIterator() -> GroupSessionJournal.Attachments.Iterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

typealias Element

The type of element this asynchronous sequence produces.

