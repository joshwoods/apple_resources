

- Create ML
- MLImageClassifier
- MLImageClassifier.ImageAugmentationOptions
-  subtract(\_:) 

Instance Method

# subtract(\_:)

Removes the elements of the given set from this set.

Create MLSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+visionOS 1.0+

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

### Combining sets

func union(Self) -> Self

Returns a new option set of the elements contained in this set, in the given set, or in both.

func formUnion(Self)

Inserts the elements of another set into this option set.

func intersection(Self) -> Self

Returns a new option set with only the elements contained in both this set and the given set.

func formIntersection(Self)

Removes all elements of this option set that are not also present in the given set.

func symmetricDifference(Self) -> Self

Returns a new option set with the elements contained in this set or in the given set, but not in both.

func formSymmetricDifference(Self)

Replaces this set with a new set containing all elements contained in either this set or the given set, but not in both.

func subtracting(Self) -> Self

Returns a new set containing the elements of this set that do not occur in the given set.

