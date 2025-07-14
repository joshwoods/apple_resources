

- RealityKit
- AnchoringComponent
- AnchoringComponent.Target
- AnchoringComponent.Target.Alignment
-  insert(\_:) 

Instance Method

# insert(\_:)

Adds the given element to the option set if it is not already a member.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
@discardableResult
mutating func insert(_ newMember: Self.Element) -> (inserted: Bool, memberAfterInsert: Self.Element)
```

Available when `Self` is `Self.Element`.

## Parameters 

`newMember`  

The element to insert.

## Return Value

`(true, newMember)` if `newMember` was not contained in `self`. Otherwise, returns `(false, oldMember)`, where `oldMember` is the member of the set equal to `newMember`.

## Discussion

In the following example, the `.secondDay` shipping option is added to the `freeOptions` option set if `purchasePrice` is greater than 50.0. For the `ShippingOptions` declaration, see the `OptionSet` protocol discussion.

```
let purchasePrice = 87.55

var freeOptions: ShippingOptions = [.standard, .priority]
if purchasePrice > 50 {
    freeOptions.insert(.secondDay)
}
print(freeOptions.contains(.secondDay))
// Prints "true"
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

func contains(Self) -> Bool

Returns a Boolean value that indicates whether a given element is a member of the option set.

func formIntersection(Self)

Removes all elements of this option set that are not also present in the given set.

func formSymmetricDifference(Self)

Replaces this set with a new set containing all elements contained in either this set or the given set, but not in both.

func formUnion(Self)

Inserts the elements of another set into this option set.

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

