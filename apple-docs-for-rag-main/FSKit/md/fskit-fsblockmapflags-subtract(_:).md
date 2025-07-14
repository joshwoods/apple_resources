

- FSKit
- FSBlockmapFlags
-  subtract(\_:) 

Instance Method

# subtract(\_:)

Removes the elements of the given set from this set.

FSKitSwiftmacOS 15.4+

``` source
mutating func subtract(_ other: Self)
```

## Parameters 

`other`  

A set of the same type as the current set.

## Discussion

In the following example, the elements of the `employees` set that are also members of the `neighbors` set are removed. In particular, the names `"Bethany"` and `"Eric"` are removed from `employees`.

```
var employees: Set = ["Alicia", "Bethany", "Chris", "Diana", "Eric"]
let neighbors: Set = ["Bethany", "Eric", "Forlani", "Greta"]
employees.subtract(neighbors)
print(employees)
// Prints "["Diana", "Chris", "Alicia"]"
```

