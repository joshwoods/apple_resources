

- RealityKit
- PhysicsJoints
-  removeAll(keepingCapacity:) 

Instance Method

# removeAll(keepingCapacity:)

Removes all elements from the collection.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
mutating func removeAll(keepingCapacity keepCapacity: Bool = false)
```

## Parameters 

`keepCapacity`  

Pass `true` to request that the collection avoid releasing its storage. Retaining the collection’s storage can be a useful optimization when you’re planning to grow the collection again. The default value is `false`.

## Discussion

Calling this method may invalidate any existing indices for use with this collection.

Complexity

O(*n*), where *n* is the length of the collection.

