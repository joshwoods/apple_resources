

- RealityKit
- CollisionGroup
-  union(\_:) 

Instance Method

# union(\_:)

Returns a new option set of the elements contained in this set, in the given set, or in both.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

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

### Option set

let rawValue: UInt32

The corresponding value of the raw type.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

typealias Element

The element type of the option set.

var isEmpty: Bool

A Boolean value that indicates whether the set has no elements.

let rawValue: UInt32

The corresponding value of the raw type.

func contains(Self) -> Bool

Returns a Boolean value that indicates whether a given element is a member of the option set.

func formIntersection(Self)

Removes all elements of this option set that are not also present in the given set.

func formSymmetricDifference(Self)

Replaces this set with a new set containing all elements contained in either this set or the given set, but not in both.

func formUnion(Self)

Inserts the elements of another set into this option set.

func insert(Self.Element) -> (inserted: Bool, memberAfterInsert: Self.Element)

Adds the given element to the option set if it is not already a member.

func intersection(Self) -> Self

Returns a new option set with only the elements contained in both this set and the given set.

func isDisjoint(with: Self) -> Bool

Returns a Boolean value that indicates whether the set has no members in common with the given set.

func isStrictSubset(of: Self) -> Bool

Returns a Boolean value that indicates whether this set is a strict subset of the given set.

func isStrictSuperset(of: Self) -> Bool

Returns a Boolean value that indicates whether this set is a strict superset of the given set.

func isSubset(of: Self) -> Bool

Returns a Boolean value that indicates whether the set is a subset of another set.

