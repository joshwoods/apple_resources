

- RealityKit
- JointTransforms
-  first 

Instance Property

# first

The first element of the collection.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
var first: Self.Element? { get }
```

## Discussion

If the collection is empty, the value of this property is `nil`.

```
let numbers = [10, 20, 30, 40, 50]
if let firstNumber = numbers.first {
    print(firstNumber)
}
// Prints "10"
```

## See Also

### Inspecting joint transform details

var count: Int

The number of elements in the collection.

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

var publisher: Publishers.Sequence&lt;Self, Never>

var underestimatedCount: Int

A value less than or equal to the number of elements in the collection.

