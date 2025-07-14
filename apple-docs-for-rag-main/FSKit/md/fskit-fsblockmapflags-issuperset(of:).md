

- FSKit
- FSBlockmapFlags
-  isSuperset(of:) 

Instance Method

# isSuperset(of:)

Returns a Boolean value that indicates whether the set is a superset of the given set.

FSKitSwiftmacOS 15.4+

``` source
func isSuperset(of other: Self) -> Bool
```

## Parameters 

`other`  

A set of the same type as the current set.

## Return Value

`true` if the set is a superset of `other`; otherwise, `false`.

## Discussion

Set *A* is a superset of another set *B* if every member of *B* is also a member of *A*.

```
let employees: Set = ["Alicia", "Bethany", "Chris", "Diana", "Eric"]
let attendees: Set = ["Alicia", "Bethany", "Diana"]
print(employees.isSuperset(of: attendees))
// Prints "true"
```

