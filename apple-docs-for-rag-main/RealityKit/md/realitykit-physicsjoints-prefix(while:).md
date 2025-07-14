

- RealityKit
- PhysicsJoints
-  prefix(while:) 

Instance Method

# prefix(while:)

Returns a subsequence containing the initial elements until `predicate` returns `false` and skipping the remaining elements.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func prefix(while predicate: (Self.Element) throws -> Bool) rethrows -> Self.SubSequence
```

## Parameters 

`predicate`  

A closure that takes an element of the sequence as its argument and returns `true` if the element should be included or `false` if it should be excluded. Once the predicate returns `false` it will not be called again.

## Discussion

Complexity

O(*n*), where *n* is the length of the collection.

