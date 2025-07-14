

- RealityKit
- JointTransforms
-  JointTransforms.Iterator 

Type Alias

# JointTransforms.Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
typealias Iterator = IndexingIterator
```

## Discussion

By default, a collection conforms to the `Sequence` protocol by supplying `IndexingIterator` as its associated `Iterator` type.

## See Also

### Identifying joint transforms

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

An individual joint transform in the collection.

typealias Index

A position of an individual joint transform in the collection.

typealias Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

typealias SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

