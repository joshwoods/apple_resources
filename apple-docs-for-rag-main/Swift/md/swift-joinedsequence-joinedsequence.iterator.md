

- Swift
- JoinedSequence
-  JoinedSequence.Iterator 

Structure

# JoinedSequence.Iterator

An iterator that presents the elements of the sequences traversed by a base iterator, concatenated using a given separator.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Iterator
```

Available when `Base` conforms to `Sequence` and `Base.Element` conforms to `Sequence`.

## Topics

### Initializers

init&lt;Separator>(base: Base.Iterator, separator: Separator)

Creates an iterator that presents the elements of `base` sequences concatenated using `separator`.

### Default Implementations

IteratorProtocol Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `Base` conforms to `Sequence` and `Base.Element` conforms to `Sequence`.

- IteratorProtocol

  Conforms when `Base` conforms to `Sequence` and `Base.Element` conforms to `Sequence`.

- Sendable

  Conforms when `Base` conforms to `Sequence`, `Base.Element` conforms to `Sequence`, `Base.Iterator` conforms to `Sendable`, `Base.Element.Element` conforms to `Sendable`, and `Base.Element.Iterator` conforms to `Sendable`.

