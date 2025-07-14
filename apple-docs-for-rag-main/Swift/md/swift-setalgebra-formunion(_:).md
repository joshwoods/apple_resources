

- Swift
- SetAlgebra
-  formUnion(\_:) 

Instance Method

# formUnion(\_:)

Adds the elements of the given set to the set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func formUnion(_ other: Self)
```

**Required** Default implementation provided.

## Parameters 

`other`  

A set of the same type as the current set.

## Discussion

In the following example, the elements of the `visitors` set are added to the `attendees` set:

```
var attendees: Set = ["Alicia", "Bethany", "Diana"]
let visitors: Set = ["Diana", "Marcia", "Nathaniel"]
attendees.formUnion(visitors)
print(attendees)
// Prints "["Diana", "Nathaniel", "Bethany", "Alicia", "Marcia"]"
```

If the set already contains one or more elements that are also in `other`, the existing members are kept.

```
var initialIndices = Set(0..

## Default Implementations

### SetAlgebra Implementations

func formUnion(Self)

Inserts the elements of another set into this option set.

## See Also

### Combining Sets

func union(Self) -> Self

Returns a new set with the elements of both this and the given set.

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

