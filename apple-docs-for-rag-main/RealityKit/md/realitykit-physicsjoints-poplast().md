

- RealityKit
- PhysicsJoints
-  popLast() 

Instance Method

# popLast()

Removes and returns the last element of the collection.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
mutating func popLast() -> Self.Element?
```

Available when `Self` conforms to `BidirectionalCollection`.

## Return Value

The last element of the collection if the collection is not empty; otherwise, `nil`.

## Discussion

Calling this method may invalidate all saved indices of this collection. Do not rely on a previously stored index value after altering a collection with any operation that can change its length.

Complexity

O(1)

