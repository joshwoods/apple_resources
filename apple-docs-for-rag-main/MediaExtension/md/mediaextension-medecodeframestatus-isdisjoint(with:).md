

- MediaExtension
- MEDecodeFrameStatus
-  isDisjoint(with:) 

Instance Method

# isDisjoint(with:)

Returns a Boolean value that indicates whether the set has no members in common with the given set.

MediaExtensionSwiftmacOS 15.0+

``` source
func isDisjoint(with other: Self) -> Bool
```

## Parameters 

`other`  

A set of the same type as the current set.

## Return Value

`true` if the set has no elements in common with `other`; otherwise, `false`.

## Discussion

In the following example, the `employees` set is disjoint with the `visitors` set because no name appears in both sets.

```
let employees: Set = ["Alicia", "Bethany", "Chris", "Diana", "Eric"]
let visitors: Set = ["Marcia", "Nathaniel", "Olivia"]
print(employees.isDisjoint(with: visitors))
// Prints "true"
```

