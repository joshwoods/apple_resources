

- Swift
-  FlattenSequence 

Structure

# FlattenSequence

A sequence consisting of all the elements contained in each segment contained in some `Base` sequence.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct FlattenSequence where Base : Sequence, Base.Element : Sequence
```

## Overview

The elements of this view are a concatenation of the elements of each sequence in the base.

The `joined` method is always lazy, but does not implicitly confer laziness on algorithms applied to its result. In other words, for ordinary sequences `s`:

- `s.joined()` does not create new storage

- `s.joined().map(f)` maps eagerly and returns a new array

- `s.lazy.joined().map(f)` maps lazily and returns a `LazyMapSequence`

## Topics

### Instance Methods

func formIndex(inout FlattenSequence&lt;Base>.Index, offsetBy: Int)

func formIndex(inout FlattenSequence&lt;Base>.Index, offsetBy: Int, limitedBy: FlattenSequence&lt;Base>.Index) -> Bool

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection

  Conforms when `Base` conforms to `BidirectionalCollection` and `Base.Element` conforms to `BidirectionalCollection`.

- Collection

  Conforms when `Base` conforms to `BidirectionalCollection` and `Base.Element` conforms to `BidirectionalCollection`.

- Copyable

  Conforms when `Base` conforms to `Sequence` and `Base.Element` conforms to `Sequence`.

- Sendable

  Conforms when `Base` conforms to `Sendable`, `Base` conforms to `Sequence`, and `Base.Element` conforms to `Sequence`.

- Sequence

  Conforms when `Base` conforms to `Collection` and `Base.Element` conforms to `Collection`.

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

struct JoinedSequence

A sequence that presents the elements of a base sequence of sequences concatenated using a given separator.

struct PrefixSequence

A sequence that only consumes up to `n` elements from an underlying `Base` iterator.

struct Repeated

A collection whose elements are all identical.

struct ReversedCollection

A collection that presents the elements of its base collection in reverse order.

struct StrideTo

A sequence of values formed by striding over a half-open interval.

struct StrideThrough

A sequence of values formed by striding over a closed interval.

struct UnfoldSequence

A sequence whose elements are produced via repeated applications of a closure to some mutable state.

struct Zip2Sequence

A sequence of pairs built out of two underlying sequences.

