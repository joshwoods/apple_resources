

- Swift
-  UnfoldSequence 

Structure

# UnfoldSequence

A sequence whose elements are produced via repeated applications of a closure to some mutable state.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct UnfoldSequence
```

## Overview

The elements of the sequence are computed lazily and the sequence may potentially be infinite in length.

Instances of `UnfoldSequence` are created with the functions `sequence(first:next:)` and `sequence(state:next:)`.

## Topics

### Type Aliases

typealias UnfoldFirstSequence

The return type of `sequence(first:next:)`.

typealias Iterator

A type that provides the sequence’s iteration interface and encapsulates its iteration state.

### Instance Methods

func next() -> Element?

Advances to the next element and returns it, or `nil` if no next element exists.

### Default Implementations

Sequence Implementations

## Relationships

### Conforms To

- IteratorProtocol
- Sendable

  Conforms when `Element` conforms to `Copyable`, `Element` conforms to `Escapable`, `Element` conforms to `Sendable`, `State` conforms to `Copyable`, `State` conforms to `Escapable`, and `State` conforms to `Sendable`.

- Sequence

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

struct ReversedCollection

A collection that presents the elements of its base collection in reverse order.

struct StrideTo

A sequence of values formed by striding over a half-open interval.

struct StrideThrough

A sequence of values formed by striding over a closed interval.

struct Zip2Sequence

A sequence of pairs built out of two underlying sequences.

