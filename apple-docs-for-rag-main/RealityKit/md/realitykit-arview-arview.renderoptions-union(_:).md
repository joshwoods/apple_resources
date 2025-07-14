

- RealityKit
- ARView
- ARView.RenderOptions
-  union(\_:) 

Instance Method

# union(\_:)

Returns a new option set of the elements contained in this set, in the given set, or in both.

RealityKitSwiftiOSiPadOSMac Catalyst

``` source
func union(_ other: Self) -> Self
```

## Parameters 

`other`  

An option set.

## Return Value

A new option set made up of the elements contained in this set, in `other`, or in both.

## Discussion

This example uses the `union(_:)` method to add two more shipping options to the default set.

```
let defaultShipping = ShippingOptions.standard
let memberShipping = defaultShipping.union([.secondDay, .priority])
print(memberShipping.contains(.priority))
// Prints "true"
```

## See Also

### Combining options

func formUnion(Self)

Inserts the elements of another set into this option set.

func intersection(Self) -> Self

Returns a new option set with only the elements contained in both this set and the given set.

func formIntersection(Self)

Removes all elements of this option set that are not also present in the given set.

func symmetricDifference(Self) -> Self

Returns a new option set with the elements contained in this set or in the given set, but not in both.

func formSymmetricDifference(Self)

Replaces this set with a new set containing all elements contained in either this set or the given set, but not in both.

