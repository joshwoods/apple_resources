

- RealityKit
- Entity
- Entity.ChildCollection
-  count 

Instance Property

# count

The number of elements in the collection.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
var count: Int { get }
```

## Discussion

To check whether a collection is empty, use its `isEmpty` property instead of comparing `count` to zero. Unless the collection guarantees random-access performance, calculating `count` can be an O(*n*) operation.

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*n*), where *n* is the length of the collection.

## See Also

### Counting entities

var isEmpty: Bool

A Boolean value indicating whether the collection is empty.

