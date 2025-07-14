

- RealityKit
- CollisionGroup
-  update(with:) 

Instance Method

# update(with:)

Inserts the given element into the set.

RealityKitSwiftiOSiPadOSMac CatalystmacOSvisionOS

``` source
@discardableResult
mutating func update(with newMember: Self.Element) -> Self.Element?
```

Available when `Self` is `Self.Element`.

## Return Value

The intersection of `[newMember]` and the set if the intersection was nonempty; otherwise, `nil`.

## Discussion

If `newMember` is not contained in the set but subsumes current members of the set, the subsumed members are returned.

```
var options: ShippingOptions = [.secondDay, .priority]
let replaced = options.update(with: .express)
print(replaced == .secondDay)
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

