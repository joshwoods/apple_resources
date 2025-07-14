

- Swift
-  LazyDropWhileSequence 

Structure

# LazyDropWhileSequence

A sequence whose elements consist of the elements that follow the initial consecutive elements of some base sequence that satisfy a given predicate.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@frozen
struct LazyDropWhileSequence where Base : Sequence
```

## Topics

### Type Aliases

typealias Element

A type representing the sequence’s elements.

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

  Conforms when `Base` conforms to `Collection`.

- Copyable

  Conforms when `Base` conforms to `Sequence`.

- LazyCollectionProtocol

  Conforms when `Base` conforms to `Collection`.

- LazySequenceProtocol

  Conforms when `Base` conforms to `Sequence`.

- Sequence

  Conforms when `Base` conforms to `Collection`.

## See Also

### Lazy Wrappers

struct LazySequence

A sequence containing the same elements as a `Base` sequence, but on which some operations such as `map` and `filter` are implemented lazily.

struct LazyMapSequence

A `Sequence` whose elements consist of those in a `Base` `Sequence` passed through a transform function returning `Element`. These elements are computed lazily, each time they’re read, by calling the transform function on a base element.

struct LazyFilterSequence

A sequence whose elements consist of the elements of some base sequence that also satisfy a given predicate.

struct LazyPrefixWhileSequence

A sequence whose elements consist of the initial consecutive elements of some base sequence that satisfy a given predicate.

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

