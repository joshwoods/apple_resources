

- RealityKit
- AnchoringComponent
- AnchoringComponent.Target
- AnchoringComponent.Target.Alignment
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value that indicates whether a given element is a member of the option set.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
func contains(_ member: Self) -> Bool
```

Available when `Self` is `Self.Element`.

## Parameters 

`member`  

The element to look for in the option set.

## Return Value

`true` if the option set contains `member`; otherwise, `false`.

## Discussion

This example uses the `contains(_:)` method to check whether next-day shipping is in the `availableOptions` instance.

```
let availableOptions = ShippingOptions.express
if availableOptions.contains(.nextDay) {
    print("Next day shipping available")
}
// Prints "Next day shipping available"
```

## See Also

### Option set conformance

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

The element type of the option set.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

var isEmpty: Bool

A Boolean value that indicates whether the set has no elements.

let rawValue: UInt8

The corresponding value of the raw type.

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

