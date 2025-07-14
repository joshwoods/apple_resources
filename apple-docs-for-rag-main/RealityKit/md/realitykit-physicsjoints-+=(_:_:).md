

- RealityKit
- PhysicsJoints
-  +=(\_:\_:) 

Operator

# +=(\_:\_:)

Appends the elements of a sequence to a range-replaceable collection.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
static func += (lhs: inout Self, rhs: Other) where Other : Sequence, Self.Element == Other.Element
```

## Parameters 

`lhs`  

The array to append to.

`rhs`  

A collection or finite sequence.

## Discussion

Use this operator to append the elements of a sequence to the end of range-replaceable collection with same `Element` type. This example appends the elements of a `Range` instance to an array of integers.

```
var numbers = [1, 2, 3, 4, 5]
numbers += 10...15
print(numbers)
// Prints "[1, 2, 3, 4, 5, 10, 11, 12, 13, 14, 15]"
```

Complexity

O(*m*), where *m* is the length of the right-hand-side argument.

