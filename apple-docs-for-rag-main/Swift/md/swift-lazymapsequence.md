

- Swift
-  LazyMapSequence 

Structure

# LazyMapSequence

A `Sequence` whose elements consist of those in a `Base` `Sequence` passed through a transform function returning `Element`. These elements are computed lazily, each time they’re read, by calling the transform function on a base element.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct LazyMapSequence where Base : Sequence
```

## Topics

### Instance Methods

func map&lt;ElementOfResult>((Element) -> ElementOfResult) -> LazyMapSequence&lt;Base, ElementOfResult>

func map&lt;ElementOfResult>((Element) -> ElementOfResult) -> LazyMapCollection&lt;Base, ElementOfResult>

### Type Aliases

typealias Elements

A `Sequence` that can contain the same elements as this one, possibly with a simpler type.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

LazySequenceProtocol Implementations

RandomAccessCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection

  Conforms when `Base` conforms to `BidirectionalCollection`, `Element` conforms to `Copyable`, and `Element` conforms to `Escapable`.

- Collection

  Conforms when `Base` conforms to `RandomAccessCollection`, `Element` conforms to `Copyable`, and `Element` conforms to `Escapable`.

- Copyable

  Conforms when `Base` conforms to `Sequence`, `Element` conforms to `Copyable`, and `Element` conforms to `Escapable`.

- LazyCollectionProtocol

  Conforms when `Base` conforms to `Collection`, `Element` conforms to `Copyable`, and `Element` conforms to `Escapable`.

- LazySequenceProtocol

  Conforms when `Base` conforms to `Sequence`, `Element` conforms to `Copyable`, and `Element` conforms to `Escapable`.

- RandomAccessCollection

  Conforms when `Base` conforms to `RandomAccessCollection`, `Element` conforms to `Copyable`, and `Element` conforms to `Escapable`.

- Sequence

  Conforms when `Base` conforms to `RandomAccessCollection`, `Element` conforms to `Copyable`, and `Element` conforms to `Escapable`.

## See Also

### Lazy Wrappers

struct LazySequence

A sequence containing the same elements as a `Base` sequence, but on which some operations such as `map` and `filter` are implemented lazily.

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

