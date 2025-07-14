

- Swift
- SetAlgebra
-  isSuperset(of:) 

Instance Method

# isSuperset(of:)

Returns a Boolean value that indicates whether the set is a superset of the given set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isSuperset(of other: Self) -> Bool
```

**Required** Default implementation provided.

## Parameters 

`other`  

A set of the same type as the current set.

## Return Value

`true` if the set is a superset of `possibleSubset`; otherwise, `false`.

## Discussion

Set *A* is a superset of another set *B* if every member of *B* is also a member of *A*.

```
let employees: Set = ["Alicia", "Bethany", "Chris", "Diana", "Eric"]
let attendees: Set = ["Alicia", "Bethany", "Diana"]
print(employees.isSuperset(of: attendees))
// Prints "true"
```

## Default Implementations

### SetAlgebra Implementations

func isSuperset(of: Self) -> Bool

Returns a Boolean value that indicates whether the set is a superset of the given set.

