

- Create ML
- MLActionClassifier
- MLActionClassifier.VideoAugmentationOptions
-  subtracting(\_:) 

Instance Method

# subtracting(\_:)

Returns a new set containing the elements of this set that do not occur in the given set.

Create MLSwiftmacOS 10.14+

``` source
func subtracting(_ other: Self) -> Self
```

## Parameters 

`other`  

A set of the same type as the current set.

## Return Value

A new set.

## Discussion

In the following example, the `nonNeighbors` set is made up of the elements of the `employees` set that are not elements of `neighbors`:

```
let employees: Set = ["Alicia", "Bethany", "Chris", "Diana", "Eric"]
let neighbors: Set = ["Bethany", "Eric", "Forlani", "Greta"]
let nonNeighbors = employees.subtracting(neighbors)
print(nonNeighbors)
// Prints "["Diana", "Chris", "Alicia"]"
```

## See Also

### Removing options

func remove(Self.Element) -> Self.Element?

Removes the given element and all elements subsumed by it.

func subtract(Self)

Removes the elements of the given set from this set.

