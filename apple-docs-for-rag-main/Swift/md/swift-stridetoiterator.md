

- Swift
-  StrideToIterator 

Structure

# StrideToIterator

An iterator for a `StrideTo` instance.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct StrideToIterator where Element : Strideable
```

## Topics

### Default Implementations

IteratorProtocol Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `Element` conforms to `Strideable`.

- IteratorProtocol

  Conforms when `Element` conforms to `Strideable`.

- Sendable

  Conforms when `Element` conforms to `Sendable`, `Element` conforms to `Strideable`, and `Element.Stride` conforms to `Sendable`.

## See Also

### Indices and Iterators

struct IteratorSequence

A sequence built around an iterator of type `Base`.

struct IndexingIterator

A type that iterates over a collection using its indices.

typealias EnumeratedIterator

typealias SetIterator

struct StrideThroughIterator

An iterator for a `StrideThrough` instance.

