

- Swift
- SetAlgebra
-  symmetricDifference(\_:) 

Instance Method

# symmetricDifference(\_:)

Returns a new set with the elements that are either in this set or in the given set, but not in both.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func symmetricDifference(_ other: Self) -> Self
```

**Required** Default implementation provided.

## Parameters 

`other`  

A set of the same type as the current set.

## Return Value

A new set.

## Discussion

In the following example, the `eitherNeighborsOrEmployees` set is made up of the elements of the `employees` and `neighbors` sets that are not in both `employees` *and* `neighbors`. In particular, the names `"Bethany"` and `"Eric"` do not appear in `eitherNeighborsOrEmployees`.

```
let employees: Set = ["Alicia", "Bethany", "Diana", "Eric"]
let neighbors: Set = ["Bethany", "Eric", "Forlani"]
let eitherNeighborsOrEmployees = employees.symmetricDifference(neighbors)
print(eitherNeighborsOrEmployees)
// Prints "["Diana", "Forlani", "Alicia"]"
```

## Default Implementations

### SetAlgebra Implementations

func symmetricDifference(Self) -> Self

Returns a new option set with the elements contained in this set or in the given set, but not in both.

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

func formSymmetricDifference(Self)

Removes the elements of the set that are also in the given set and adds the members of the given set that are not already in the set.

**Required** Default implementation provided.

