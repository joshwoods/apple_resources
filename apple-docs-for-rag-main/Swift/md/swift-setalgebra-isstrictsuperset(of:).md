

- Swift
- SetAlgebra
-  isStrictSuperset(of:) 

Instance Method

# isStrictSuperset(of:)

Returns a Boolean value that indicates whether this set is a strict superset of the given set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

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

### Comparing Sets

func isStrictSubset(of: Self) -> Bool

Returns a Boolean value that indicates whether this set is a strict subset of the given set.

