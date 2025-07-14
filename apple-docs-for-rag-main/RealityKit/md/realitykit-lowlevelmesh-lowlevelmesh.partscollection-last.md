

- RealityKit
- LowLevelMesh
- LowLevelMesh.PartsCollection
-  last 

Instance Property

# last

The last element of the collection.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
var last: Self.Element? { get }
```

## Discussion

If the collection is empty, the value of this property is `nil`.

```
let numbers = [10, 20, 30, 40, 50]
if let lastNumber = numbers.last {
    print(lastNumber)
}
// Prints "50"
```

Complexity

O(1)

