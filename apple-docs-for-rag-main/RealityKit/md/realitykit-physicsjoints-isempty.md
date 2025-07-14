

- RealityKit
- PhysicsJoints
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

