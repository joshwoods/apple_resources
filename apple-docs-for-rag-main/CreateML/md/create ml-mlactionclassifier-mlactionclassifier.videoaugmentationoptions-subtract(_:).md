

- Create ML
- MLActionClassifier
- MLActionClassifier.VideoAugmentationOptions
-  subtract(\_:) 

Instance Method

# subtract(\_:)

Removes the elements of the given set from this set.

Create MLSwiftmacOS 10.14+

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

## See Also

### Removing options

func remove(Self.Element) -> Self.Element?

Removes the given element and all elements subsumed by it.

func subtracting(Self) -> Self

Returns a new set containing the elements of this set that do not occur in the given set.

