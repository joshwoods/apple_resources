

- Swift
- CollectionDifference
-  CollectionDifference.Iterator 

Type Alias

# CollectionDifference.Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
typealias Iterator = IndexingIterator>
```

## Discussion

By default, a collection conforms to the `Sequence` protocol by supplying `IndexingIterator` as its associated `Iterator` type.

