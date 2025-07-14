

- RealityKit
- JointTransforms
-  isEmpty 

Instance Property

# isEmpty

A Boolean value indicating whether the collection is empty.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
var isEmpty: Bool { get }
```

## Discussion

When you need to check whether your collection is empty, use the `isEmpty` property instead of checking that the `count` property is equal to zero. For collections that don’t conform to `RandomAccessCollection`, accessing the `count` property iterates through the elements of the collection.

```
let horseName = "Silver"
if horseName.isEmpty {
    print("My horse has no name.")
} else {
    print("Hi ho, \(horseName)!")
}
// Prints "Hi ho, Silver!")
```

Complexity

O(1)

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

var last: Self.Element?

The last element of the collection.

var lazy: LazySequence&lt;Self>

A sequence containing the same elements as this sequence, but on which some operations, such as `map` and `filter`, are implemented lazily.

var publisher: Publishers.Sequence&lt;Self, Never>

var underestimatedCount: Int

A value less than or equal to the number of elements in the collection.

