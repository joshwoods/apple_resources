

- RealityKit
- PhysicsJoints
-  removeLast() 

Instance Method

# removeLast()

Removes and returns the last element of the collection.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
@discardableResult
mutating func removeLast() -> Self.Element
```

Available when `Self` conforms to `BidirectionalCollection`.

## Return Value

The last element of the collection.

## Discussion

The collection must not be empty.

Calling this method may invalidate all saved indices of this collection. Do not rely on a previously stored index value after altering a collection with any operation that can change its length.

Complexity

O(1)

