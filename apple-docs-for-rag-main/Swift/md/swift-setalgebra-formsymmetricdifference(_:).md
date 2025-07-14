

- Swift
- SetAlgebra
-  formSymmetricDifference(\_:) 

Instance Method

# formSymmetricDifference(\_:)

Removes the elements of the set that are also in the given set and adds the members of the given set that are not already in the set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func formSymmetricDifference(_ other: Self)
```

**Required** Default implementation provided.

## Parameters 

`other`  

A set of the same type.

## Discussion

In the following example, the elements of the `employees` set that are also members of `neighbors` are removed from `employees`, while the elements of `neighbors` that are not members of `employees` are added to `employees`. In particular, the names `"Bethany"` and `"Eric"` are removed from `employees` while the name `"Forlani"` is added.

```
var employees: Set = ["Alicia", "Bethany", "Diana", "Eric"]
let neighbors: Set = ["Bethany", "Eric", "Forlani"]
employees.formSymmetricDifference(neighbors)
print(employees)
// Prints "["Diana", "Forlani", "Alicia"]"
```

## Default Implementations

### SetAlgebra Implementations

func formSymmetricDifference(Self)

Replaces this set with a new set containing all elements contained in either this set or the given set, but not in both.

## See Also

### Combining Sets

func union(Self) -> Self

Returns a new set with the elements of both this and the given set.

**Required** Default implementation provided.

func formUnion(Self)

Adds the elements of the given set to the set.

**Required** Default implementation provided.

func intersection(Self) -> Self

Returns a new set with the elements that are common to both this set and the given set.

**Required** Default implementation provided.

func formIntersection(Self)

Removes the elements of this set that aren’t also in the given set.

**Required** Default implementation provided.

func symmetricDifference(Self) -> Self

Returns a new set with the elements that are either in this set or in the given set, but not in both.

**Required** Default implementation provided.

