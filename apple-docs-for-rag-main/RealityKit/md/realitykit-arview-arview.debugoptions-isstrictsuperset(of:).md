

- RealityKit
- ARView
- ARView.DebugOptions
-  isStrictSuperset(of:) 

Instance Method

# isStrictSuperset(of:)

Returns a Boolean value that indicates whether this set is a strict superset of the given set.

RealityKitSwiftiOSiPadOSMac CatalystmacOS

``` source
func isStrictSuperset(of other: Self) -> Bool
```

## Parameters 

`other`  

A set of the same type as the current set.

## Return Value

`true` if the set is a strict superset of `other`; otherwise, `false`.

## Discussion

Set *A* is a strict superset of another set *B* if every member of *B* is also a member of *A* and *A* contains at least one element that is *not* a member of *B*.

```
let employees: Set = ["Alicia", "Bethany", "Chris", "Diana", "Eric"]
let attendees: Set = ["Alicia", "Bethany", "Diana"]
print(employees.isStrictSuperset(of: attendees))
// Prints "true"

// A set is never a strict superset of itself:
print(employees.isStrictSuperset(of: employees))
// Prints "false"
```

## See Also

### Comparing options

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

func isSubset(of: Self) -> Bool

Returns a Boolean value that indicates whether the set is a subset of another set.

func isStrictSubset(of: Self) -> Bool

Returns a Boolean value that indicates whether this set is a strict subset of the given set.

func isSuperset(of: Self) -> Bool

Returns a Boolean value that indicates whether the set is a superset of the given set.

func isDisjoint(with: Self) -> Bool

Returns a Boolean value that indicates whether the set has no members in common with the given set.

