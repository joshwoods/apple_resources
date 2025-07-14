

- Swift
- SetAlgebra
-  formIntersection(\_:) 

Instance Method

# formIntersection(\_:)

Removes the elements of this set that aren’t also in the given set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func formIntersection(_ other: Self)
```

**Required** Default implementation provided.

## Parameters 

`other`  

A set of the same type as the current set.

## Discussion

In the following example, the elements of the `employees` set that are not also members of the `neighbors` set are removed. In particular, the names `"Alicia"`, `"Chris"`, and `"Diana"` are removed.

```
var employees: Set = ["Alicia", "Bethany", "Chris", "Diana", "Eric"]
let neighbors: Set = ["Bethany", "Eric", "Forlani", "Greta"]
employees.formIntersection(neighbors)
print(employees)
// Prints "["Bethany", "Eric"]"
```

## Default Implementations

### SetAlgebra Implementations

func formIntersection(Self)

Removes all elements of this option set that are not also present in the given set.

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

func symmetricDifference(Self) -> Self

Returns a new set with the elements that are either in this set or in the given set, but not in both.

**Required** Default implementation provided.

func formSymmetricDifference(Self)

Removes the elements of the set that are also in the given set and adds the members of the given set that are not already in the set.

**Required** Default implementation provided.

