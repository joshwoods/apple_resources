

- RealityKit
- Entity
- Entity.ComponentSet
-  formIndex(\_:offsetBy:) 

Instance Method

# formIndex(\_:offsetBy:)

Offsets the given index by the specified distance.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func formIndex(
    _ i: inout Self.Index,
    offsetBy distance: Int
)
```

## Parameters 

`i`  

A valid index of the collection.

`distance`  

The distance to offset `i`. `distance` must not be negative unless the collection conforms to the `BidirectionalCollection` protocol.

## Discussion

The value passed as `distance` must not offset `i` beyond the bounds of the collection.

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*k*), where *k* is the absolute value of `distance`.

