

- Swift
-  LazyFilterCollection 

Type Alias

# LazyFilterCollection

A lazy `Collection` wrapper that includes the elements of an underlying collection that satisfy a predicate.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
typealias LazyFilterCollection = LazyFilterSequence where T : Collection
```

## Discussion

Note

The performance of accessing `startIndex`, `first`, any methods that depend on `startIndex`, or of advancing an index depends on how sparsely the filtering predicate is satisfied, and may not offer the usual performance given by `Collection`. Be aware, therefore, that general operations on `LazyFilterCollection` instances may not have the documented complexity.

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

struct LazyDropWhileSequence

A sequence whose elements consist of the elements that follow the initial consecutive elements of some base sequence that satisfy a given predicate.

typealias LazyCollection

A collection containing the same elements as a `Base` collection, but on which some operations such as `map` and `filter` are implemented lazily.

typealias LazyDropWhileCollection

A lazy wrapper that includes the elements of an underlying collection after any initial consecutive elements that satisfy a predicate.

typealias LazyMapCollection

A `Collection` whose elements consist of those in a `Base` `Collection` passed through a transform function returning `Element`. These elements are computed lazily, each time they’re read, by calling the transform function on a base element.

typealias LazyPrefixWhileCollection

A lazy collection wrapper that includes the initial consecutive elements of an underlying collection that satisfy a predicate.

