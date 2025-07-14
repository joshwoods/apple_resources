

- RealityKit
- JointTransforms
-  publisher 

Instance Property

# publisher

RealityKitSwiftiOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
var publisher: Publishers.Sequence { get }
```

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

var endIndex: JointTransforms.Index

An index to the last joint transform in the collection.

var isEmpty: Bool

A Boolean value indicating whether the collection is empty.

var last: Self.Element?

The last element of the collection.

var lazy: LazySequence&lt;Self>

A sequence containing the same elements as this sequence, but on which some operations, such as `map` and `filter`, are implemented lazily.

var underestimatedCount: Int

A value less than or equal to the number of elements in the collection.

