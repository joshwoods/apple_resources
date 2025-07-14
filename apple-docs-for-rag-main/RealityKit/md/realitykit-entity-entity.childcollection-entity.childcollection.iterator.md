

- RealityKit
- Entity
- Entity.ChildCollection
-  Entity.ChildCollection.Iterator 

Type Alias

# Entity.ChildCollection.Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
typealias Iterator = Entity.ChildCollection.IndexingIterator
```

## Discussion

By default, a collection conforms to the `Sequence` protocol by supplying `IndexingIterator` as its associated `Iterator` type.

