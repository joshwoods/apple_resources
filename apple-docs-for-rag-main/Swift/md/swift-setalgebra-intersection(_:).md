

- Swift
- SetAlgebra
-  intersection(\_:) 

Instance Method

# intersection(\_:)

Returns a new set with the elements that are common to both this set and the given set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func intersection(_ other: Self) -> Self
```

**Required** Default implementation provided.

## Parameters 

`other`  

A set of the same type as the current set.

## Return Value

A new set.

## Discussion

In the following example, the `bothNeighborsAndEmployees` set is made up of the elements that are in *both* the `employees` and `neighbors` sets. Elements that are in only one or the other are left out of the result of the intersection.

```
let employees: Set = ["Alicia", "Bethany", "Chris", "Diana", "Eric"]
let neighbors: Set = ["Bethany", "Eric", "Forlani", "Greta"]
let bothNeighborsAndEmployees = employees.intersection(neighbors)
print(bothNeighborsAndEmployees)
// Prints "["Bethany", "Eric"]"
```

Note

If this set and `other` contain elements that are equal but distinguishable (e.g. via `===`), which of these elements is present in the result is unspecified.

## Default Implementations

### SetAlgebra Implementations

func intersection(Self) -> Self

Returns a new option set with only the elements contained in both this set and the given set.

## See Also

### Combining Sets

func union(Self) -> Self

Returns a new set with the elements of both this and the given set.

**Required** Default implementation provided.

func formUnion(Self)

Adds the elements of the given set to the set.

**Required** Default implementation provided.

func formIntersection(Self)

Removes the elements of this set that aren’t also in the given set.

**Required** Default implementation provided.

func symmetricDifference(Self) -> Self

Returns a new set with the elements that are either in this set or in the given set, but not in both.

**Required** Default implementation provided.

func formSymmetricDifference(Self)

Removes the elements of the set that are also in the given set and adds the members of the given set that are not already in the set.

**Required** Default implementation provided.

