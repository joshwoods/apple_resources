

- TabularData
- Column
-  Column.Iterator 

Type Alias

# Column.Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
typealias Iterator = IndexingIterator>
```

## Discussion

By default, a collection conforms to the `Sequence` protocol by supplying `IndexingIterator` as its associated `Iterator` type.

