

- Swift
- Swift Standard Library
- Collections
- Set
-  SetAlgebra Implementations 

API Collection

# SetAlgebra Implementations

## Topics

### Initializers

init()

Creates an empty set.

init&lt;Source>(Source)

Creates a new set from a finite sequence of items.

init&lt;S>(S)

Creates a new set from a finite sequence of items.

init(arrayLiteral: Self.Element...)

Creates a set containing the elements of the given array literal.

### Instance Methods

func contains(Element) -> Bool

Returns a Boolean value that indicates whether the given element exists in the set.

func formIntersection&lt;S>(S)

Removes the elements of the set that aren’t also in the given sequence.

func formSymmetricDifference(Set&lt;Element>)

Removes the elements of the set that are also in the given sequence and adds the members of the sequence that are not already in the set.

func formUnion&lt;S>(S)

Inserts the elements of the given sequence into the set.

func insert(Element) -> (inserted: Bool, memberAfterInsert: Element)

Inserts the given element in the set if it is not already present.

func intersection(Set&lt;Element>) -> Set&lt;Element>

Returns a new set with the elements that are common to both this set and the given sequence.

func isDisjoint(with: Set&lt;Element>) -> Bool

Returns a Boolean value that indicates whether this set has no members in common with the given set.

func isSubset(of: Set&lt;Element>) -> Bool

Returns a Boolean value that indicates whether this set is a subset of the given set.

func isSuperset(of: Set&lt;Element>) -> Bool

Returns a Boolean value that indicates whether this set is a superset of the given set.

func remove(Element) -> Element?

Removes the specified element from the set.

func subtract(Self)

Removes the elements of the given set from this set.

func subtract(Set&lt;Element>)

Removes the elements of the given set from this set.

func subtracting(Set&lt;Element>) -> Set&lt;Element>

Returns a new set containing the elements of this set that do not occur in the given set.

func symmetricDifference&lt;S>(S) -> Set&lt;Element>

Returns a new set with the elements that are either in this set or in the given sequence, but not in both.

func union&lt;S>(S) -> Set&lt;Element>

Returns a new set with the elements of both this set and the given sequence.

func update(with: Element) -> Element?

Inserts the given element into the set unconditionally.

