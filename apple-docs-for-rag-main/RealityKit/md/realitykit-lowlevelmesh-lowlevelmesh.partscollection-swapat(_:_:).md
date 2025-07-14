

- RealityKit
- LowLevelMesh
- LowLevelMesh.PartsCollection
-  swapAt(\_:\_:) 

Instance Method

# swapAt(\_:\_:)

Exchanges the values at the specified indices of the collection.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
mutating func swapAt(
    _ i: Self.Index,
    _ j: Self.Index
)
```

## Parameters 

`i`  

The index of the first value to swap.

`j`  

The index of the second value to swap.

## Discussion

Both parameters must be valid indices of the collection that are not equal to `endIndex`. Calling `swapAt(_:_:)` with the same index as both `i` and `j` has no effect.

Complexity

O(1)

