

- RealityKit
- PhysicsJoints
-  +(\_:\_:) 

Operator

# +(\_:\_:)

Creates a new collection by concatenating the elements of a sequence and a collection.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
static func + (lhs: Other, rhs: Self) -> Self where Other : Sequence, Self.Element == Other.Element
```

## Parameters 

`lhs`  

A collection or finite sequence.

`rhs`  

A range-replaceable collection.

## Discussion

The two arguments must have the same `Element` type. For example, you can concatenate the elements of a `Range` instance and an integer array.

```
let numbers = [7, 8, 9, 10]
let moreNumbers = (1...6) + numbers
print(moreNumbers)
// Prints "[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]"
```

The resulting collection has the type of argument on the right-hand side. In the example above, `moreNumbers` has the same type as `numbers`, which is `[Int]`.

