

- Swift
- SetAlgebra
-  union(\_:) 

Instance Method

# union(\_:)

Returns a new set with the elements of both this and the given set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func union(_ other: Self) -> Self
```

**Required** Default implementation provided.

## Parameters 

`other`  

A set of the same type as the current set.

## Return Value

A new set with the unique elements of this set and `other`.

## Discussion

In the following example, the `attendeesAndVisitors` set is made up of the elements of the `attendees` and `visitors` sets:

```
let attendees: Set = ["Alicia", "Bethany", "Diana"]
let visitors = ["Marcia", "Nathaniel"]
let attendeesAndVisitors = attendees.union(visitors)
print(attendeesAndVisitors)
// Prints "["Diana", "Nathaniel", "Bethany", "Alicia", "Marcia"]"
```

If the set already contains one or more elements that are also in `other`, the existing members are kept.

```
let initialIndices = Set(0..

Note

If this set and `other` contain elements that are equal but distinguishable (e.g. via `===`), which of these elements is present in the result is unspecified.

## Default Implementations

### SetAlgebra Implementations

func union(Self) -> Self

Returns a new option set of the elements contained in this set, in the given set, or in both.

## See Also

### Combining Sets

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

func formSymmetricDifference(Self)

Removes the elements of the set that are also in the given set and adds the members of the given set that are not already in the set.

**Required** Default implementation provided.

