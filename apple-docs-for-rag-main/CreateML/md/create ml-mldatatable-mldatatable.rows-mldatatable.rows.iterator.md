

- Create ML
- MLDataTable
- MLDataTable.Rows
-  MLDataTable.Rows.Iterator 

Type Alias

# MLDataTable.Rows.Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
typealias Iterator = IndexingIterator
```

## Discussion

By default, a collection conforms to the `Sequence` protocol by supplying `IndexingIterator` as its associated `Iterator` type.

