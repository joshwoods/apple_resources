

- Swift
-  IteratorSequence 

Structure

# IteratorSequence

A sequence built around an iterator of type `Base`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct IteratorSequence where Base : IteratorProtocol
```

## Overview

Useful mostly to recover the ability to use `for`…`in`, given just an iterator `i`:

```
for x in IteratorSequence(i) { ... }
```

## Topics

### Initializers

init(Base)

Creates an instance whose iterator is a copy of `base`.

### Default Implementations

IteratorProtocol Implementations

Sequence Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `Base` conforms to `IteratorProtocol`.

- IteratorProtocol

  Conforms when `Base` conforms to `IteratorProtocol`.

- Sendable

  Conforms when `Base` conforms to `IteratorProtocol` and `Sendable`.

- Sequence

  Conforms when `Base` conforms to `IteratorProtocol`.

## See Also

### Indices and Iterators

struct IndexingIterator

A type that iterates over a collection using its indices.

typealias EnumeratedIterator

typealias SetIterator

struct StrideThroughIterator

An iterator for a `StrideThrough` instance.

struct StrideToIterator

An iterator for a `StrideTo` instance.

