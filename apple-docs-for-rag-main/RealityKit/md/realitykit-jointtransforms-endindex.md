

- RealityKit
- JointTransforms
-  endIndex 

Instance Property

# endIndex

An index to the last joint transform in the collection.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var endIndex: JointTransforms.Index { get }
```

## Discussion

For more more on the sequence’s final index, see endIndex.

## See Also

### Inspecting joint transform details

var count: Int

The number of elements in the collection.

var first: Self.Element?

The first element of the collection.

var indices: DefaultIndices&lt;Self>

The indices that are valid for subscripting the collection, in ascending order.

var startIndex: JointTransforms.Index

An index to the first joint transform in the collection.

var isEmpty: Bool

A Boolean value indicating whether the collection is empty.

var last: Self.Element?

The last element of the collection.

var lazy: LazySequence&lt;Self>

A sequence containing the same elements as this sequence, but on which some operations, such as `map` and `filter`, are implemented lazily.

var publisher: Publishers.Sequence&lt;Self, Never>

var underestimatedCount: Int

A value less than or equal to the number of elements in the collection.

