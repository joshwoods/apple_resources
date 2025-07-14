

- RealityKit
- PhysicsJoints
-  removeFirst() 

Instance Method

# removeFirst()

Removes and returns the first element of the collection.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
@discardableResult
mutating func removeFirst() -> Self.Element
```

## Return Value

The removed element.

## Discussion

The collection must not be empty.

```
var bugs = ["Aphid", "Bumblebee", "Cicada", "Damselfly", "Earwig"]
bugs.removeFirst()
print(bugs)
// Prints "["Bumblebee", "Cicada", "Damselfly", "Earwig"]"
```

Calling this method may invalidate any existing indices for use with this collection.

Complexity

O(*n*), where *n* is the length of the collection.

