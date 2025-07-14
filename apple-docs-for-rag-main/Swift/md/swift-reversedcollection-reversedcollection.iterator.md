

- Swift
- ReversedCollection
-  ReversedCollection.Iterator 

Structure

# ReversedCollection.Iterator

A type that provides the sequence’s iteration interface and encapsulates its iteration state.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Iterator
```

Available when `Base` conforms to `BidirectionalCollection`.

## Topics

### Default Implementations

IteratorProtocol Implementations

Sequence Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `Base` conforms to `BidirectionalCollection`.

- IteratorProtocol

  Conforms when `Base` conforms to `BidirectionalCollection`.

- Sendable

  Conforms when `Base` conforms to `BidirectionalCollection`, `Base` conforms to `Sendable`, and `Base.Index` conforms to `Sendable`.

- Sequence

  Conforms when `Base` conforms to `BidirectionalCollection`.

