

- SwiftData
- FetchResultsCollection
-  FetchResultsCollection.Iterator 

Type Alias

# FetchResultsCollection.Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
typealias Iterator = IndexingIterator>
```

## Discussion

By default, a collection conforms to the `Sequence` protocol by supplying `IndexingIterator` as its associated `Iterator` type.

