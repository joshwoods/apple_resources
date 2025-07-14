

- System
- FileDescriptor
- FileDescriptor.OpenOptions
-  SetAlgebra Implementations 

API Collection

# SetAlgebra Implementations

## Topics

### Initializers

init&lt;S>(S)

Creates a new set from a finite sequence of items.

init(arrayLiteral: Self.Element...)

Creates a set containing the elements of the given array literal.

### Instance Properties

var isEmpty: Bool

A Boolean value that indicates whether the set has no elements.

### Instance Methods

func isDisjoint(with: Self) -> Bool

Returns a Boolean value that indicates whether the set has no members in common with the given set.

func isStrictSubset(of: Self) -> Bool

Returns a Boolean value that indicates whether this set is a strict subset of the given set.

func isStrictSuperset(of: Self) -> Bool

Returns a Boolean value that indicates whether this set is a strict superset of the given set.

func isSubset(of: Self) -> Bool

Returns a Boolean value that indicates whether the set is a subset of another set.

func isSuperset(of: Self) -> Bool

Returns a Boolean value that indicates whether the set is a superset of the given set.

func subtract(Self)

Removes the elements of the given set from this set.

func subtracting(Self) -> Self

Returns a new set containing the elements of this set that do not occur in the given set.

