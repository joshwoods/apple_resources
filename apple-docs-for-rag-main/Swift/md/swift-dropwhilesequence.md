

- Swift
-  DropWhileSequence 

Structure

# DropWhileSequence

A sequence that lazily consumes and drops `n` elements from an underlying `Base` iterator before possibly returning the first available element.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct DropWhileSequence where Base : Sequence
```

## Overview

The underlying iterator’s sequence may be infinite.

## Topics

### Instance Methods

func drop(while: (DropWhileSequence&lt;Base>.Element) throws -> Bool) rethrows -> DropWhileSequence&lt;Base>

### Type Aliases

typealias Element

A type representing the sequence’s elements.

### Default Implementations

Sequence Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `Base` conforms to `Sequence`.

- Sendable

  Conforms when `Base` conforms to `Sequence`, `Base.Element` conforms to `Sendable`, and `Base.Iterator` conforms to `Sendable`.

- Sequence

  Conforms when `Base` conforms to `Sequence`.

## See Also

### Wrappers for Algorithms

struct CollectionDifference

A collection of insertions and removals that describe the difference between two ordered collection states.

struct DropFirstSequence

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

