

- Swift
- Swift Standard Library
- Collections
-  Supporting Types 

API Collection

# Supporting Types

Use wrappers, indices, and iterators in operations like slicing, flattening, and reversing a collection.

## Topics

### Slices

struct Slice

A view into a subsequence of elements of another collection.

### Range Expressions

struct PartialRangeUpTo

A partial half-open interval up to, but not including, an upper bound.

struct PartialRangeThrough

A partial interval up to, and including, an upper bound.

struct PartialRangeFrom

A partial interval extending upward from a lower bound.

protocol RangeExpression

A type that can be used to slice a collection.

enum UnboundedRange_

A range expression that represents the entire range of a collection.

### Type-Erasing Wrappers

struct AnySequence

A type-erased sequence.

struct AnyCollection

A type-erased wrapper over any collection with indices that support forward traversal.

struct AnyBidirectionalCollection

A type-erased wrapper over any collection with indices that support bidirectional traversal.

struct AnyRandomAccessCollection

A type-erased wrapper over any collection with indices that support random access traversal.

struct AnyIterator

A type-erased iterator of `Element`.

struct AnyIndex

A wrapper over an underlying index that hides the specific underlying type.

struct AnyHashable

A type-erased hashable value.

### Lazy Wrappers

Use these lazy wrappers to defer any filtering or transformation of collection elements until elements are accessed.

struct LazySequence

A sequence containing the same elements as a `Base` sequence, but on which some operations such as `map` and `filter` are implemented lazily.

struct LazyMapSequence

A `Sequence` whose elements consist of those in a `Base` `Sequence` passed through a transform function returning `Element`. These elements are computed lazily, each time they’re read, by calling the transform function on a base element.

struct LazyFilterSequence

A sequence whose elements consist of the elements of some base sequence that also satisfy a given predicate.

struct LazyPrefixWhileSequence

A sequence whose elements consist of the initial consecutive elements of some base sequence that satisfy a given predicate.

struct LazyDropWhileSequence

A sequence whose elements consist of the elements that follow the initial consecutive elements of some base sequence that satisfy a given predicate.

typealias LazyCollection

A collection containing the same elements as a `Base` collection, but on which some operations such as `map` and `filter` are implemented lazily.

typealias LazyDropWhileCollection

A lazy wrapper that includes the elements of an underlying collection after any initial consecutive elements that satisfy a predicate.

typealias LazyFilterCollection

A lazy `Collection` wrapper that includes the elements of an underlying collection that satisfy a predicate.

typealias LazyMapCollection

A `Collection` whose elements consist of those in a `Base` `Collection` passed through a transform function returning `Element`. These elements are computed lazily, each time they’re read, by calling the transform function on a base element.

typealias LazyPrefixWhileCollection

A lazy collection wrapper that includes the initial consecutive elements of an underlying collection that satisfy a predicate.

### Wrappers for Algorithms

Many collection operations are performed by wrapping a collection in another type, instead of copying the collection’s contents.

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

struct Zip2Sequence

A sequence of pairs built out of two underlying sequences.

### Collections of Indices

struct DefaultIndices

A collection of indices for an arbitrary collection

### Indices and Iterators

Index and iterator types for other sequence and collection types in the standard library.

struct IteratorSequence

A sequence built around an iterator of type `Base`.

struct IndexingIterator

A type that iterates over a collection using its indices.

typealias EnumeratedIterator

typealias SetIterator

struct StrideThroughIterator

An iterator for a `StrideThrough` instance.

struct StrideToIterator

An iterator for a `StrideTo` instance.

### Deprecated

typealias DictionaryIndex

typealias SetIndex

typealias CountableClosedRange

typealias CountablePartialRangeFrom

typealias CountableRange

## See Also

### Advanced Collection Topics

Sequence and Collection Protocols

Write generic code that works with any collection, or build your own collection types.

Managed Buffers

Build your own buffer-backed collection types.

