

- Swift
-  ReversedCollection 

Structure

# ReversedCollection

A collection that presents the elements of its base collection in reverse order.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct ReversedCollection where Base : BidirectionalCollection
```

## Overview

Note

This type is the result of `x.reversed()` where `x` is a collection having bidirectional indices.

The `reversed()` method is always lazy when applied to a collection with bidirectional indices, but does not implicitly confer laziness on algorithms applied to its result. In other words, for ordinary collections `c` having bidirectional indices:

- `c.reversed()` does not create new storage

- `c.reversed().map(f)` maps eagerly and returns a new array

- `c.lazy.reversed().map(f)` maps lazily and returns a `LazyMapCollection`

## Topics

### Instance Methods

func reversed() -> Base

Reversing a reversed collection returns the original collection.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

LazySequenceProtocol Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection

  Conforms when `Base` conforms to `BidirectionalCollection`.

- Collection

  Conforms when `Base` conforms to `RandomAccessCollection`.

- Copyable

  Conforms when `Base` conforms to `BidirectionalCollection` and `LazySequenceProtocol`.

- LazySequenceProtocol

  Conforms when `Base` conforms to `BidirectionalCollection` and `LazySequenceProtocol`.

- RandomAccessCollection

  Conforms when `Base` conforms to `RandomAccessCollection`.

- Sendable

  Conforms when `Base` conforms to `BidirectionalCollection` and `Sendable`.

- Sequence

  Conforms when `Base` conforms to `BidirectionalCollection` and `LazySequenceProtocol`.

## See Also

### Wrappers for Algorithms

struct CollectionDifference

A collection of insertions and removals that describe the difference between two ordered collection states.

struct DropFirstSequence

A sequence that lazily consumes and drops `n` elements from an underlying `Base` iterator before possibly returning the first available element.

struct DropWhileSequence

A sequence that lazily consumes and drops `n` elements from an underlying `Base` iterator before possibly returning the first available element.

struct EnumeratedSequence

An enumeration of the elements of a sequence or collection.

typealias FlattenCollection

struct FlattenSequence

A sequence consisting of all the elements contained in each segment contained in some `Base` sequence.

struct JoinedSequence

A sequence that presents the elements of a base sequence of sequences concatenated using a given separator.

struct PrefixSequence

A sequence that only consumes up to `n` elements from an underlying `Base` iterator.

struct Repeated

A collection whose elements are all identical.

struct StrideTo

A sequence of values formed by striding over a half-open interval.

struct StrideThrough

A sequence of values formed by striding over a closed interval.

struct UnfoldSequence

A sequence whose elements are produced via repeated applications of a closure to some mutable state.

struct Zip2Sequence

A sequence of pairs built out of two underlying sequences.

