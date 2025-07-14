

- Swift
-  Zip2Sequence 

Structure

# Zip2Sequence

A sequence of pairs built out of two underlying sequences.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct Zip2Sequence where Sequence1 : Sequence, Sequence2 : Sequence
```

## Overview

In a `Zip2Sequence` instance, the elements of the *i*th pair are the *i*th elements of each underlying sequence. To create a `Zip2Sequence` instance, use the `zip(_:_:)` function.

The following example uses the `zip(_:_:)` function to iterate over an array of strings and a countable range at the same time:

```
let words = ["one", "two", "three", "four"]
let numbers = 1...4

for (word, number) in zip(words, numbers) {
    print("\(word): \(number)")
}
// Prints "one: 1"
// Prints "two: 2"
// Prints "three: 3"
// Prints "four: 4"
```

## Topics

### Type Aliases

typealias Stream1

typealias Stream2

### Default Implementations

Sequence Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `Sequence1` conforms to `Sequence` and `Sequence2` conforms to `Sequence`.

- Sendable

  Conforms when `Sequence1` conforms to `Sendable`, `Sequence1` conforms to `Sequence`, `Sequence2` conforms to `Sendable`, and `Sequence2` conforms to `Sequence`.

- Sequence

  Conforms when `Sequence1` conforms to `Sequence` and `Sequence2` conforms to `Sequence`.

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

struct UnfoldSequence

A sequence whose elements are produced via repeated applications of a closure to some mutable state.

