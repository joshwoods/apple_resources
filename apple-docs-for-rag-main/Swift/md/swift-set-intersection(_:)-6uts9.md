

- Swift
- Set
-  intersection(\_:) 

Instance Method

# intersection(\_:)

Returns a new set with the elements that are common to both this set and the given sequence.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func intersection(_ other: S) -> Set where Element == S.Element, S : Sequence
```

Available when `Element` conforms to `Hashable`.

## Parameters 

`other`  

A sequence of elements. `other` must be finite.

## Return Value

A new set.

## Discussion

In the following example, the `bothNeighborsAndEmployees` set is made up of the elements that are in *both* the `employees` and `neighbors` sets. Elements that are in only one or the other are left out of the result of the intersection.

```
let employees: Set = ["Alicia", "Bethany", "Chris", "Diana", "Eric"]
let neighbors = ["Bethany", "Eric", "Forlani", "Greta"]
let bothNeighborsAndEmployees = employees.intersection(neighbors)
print(bothNeighborsAndEmployees)
// Prints "["Bethany", "Eric"]"
```

## See Also

### Combining Sets

func union&lt;S>(S) -> Set&lt;Element>

Returns a new set with the elements of both this set and the given sequence.

func formUnion&lt;S>(S)

Inserts the elements of the given sequence into the set.

func intersection(Set&lt;Element>) -> Set&lt;Element>

Returns a new set with the elements that are common to both this set and the given sequence.

func formIntersection&lt;S>(S)

Removes the elements of the set that aren’t also in the given sequence.

func symmetricDifference&lt;S>(S) -> Set&lt;Element>

Returns a new set with the elements that are either in this set or in the given sequence, but not in both.

func formSymmetricDifference(Set&lt;Element>)

Removes the elements of the set that are also in the given sequence and adds the members of the sequence that are not already in the set.

func formSymmetricDifference&lt;S>(S)

Replace this set with the elements contained in this set or the given set, but not both.

func subtract(Set&lt;Element>)

Removes the elements of the given set from this set.

func subtract&lt;S>(S)

Removes the elements of the given sequence from the set.

func subtracting(Set&lt;Element>) -> Set&lt;Element>

Returns a new set containing the elements of this set that do not occur in the given set.

func subtracting&lt;S>(S) -> Set&lt;Element>

Returns a new set containing the elements of this set that do not occur in the given sequence.

