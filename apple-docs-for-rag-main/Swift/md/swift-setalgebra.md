

- Swift
-  SetAlgebra 

Protocol

# SetAlgebra

A type that provides mathematical set operations.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol SetAlgebra : Equatable, ExpressibleByArrayLiteral
```

## Overview

You use types that conform to the `SetAlgebra` protocol when you need efficient membership tests or mathematical set operations such as intersection, union, and subtraction. In the standard library, you can use the `Set` type with elements of any hashable type, or you can easily create bit masks with `SetAlgebra` conformance using the `OptionSet` protocol. See those types for more information.

Note

Unlike ordinary set types, the `Element` type of an `OptionSet` is identical to the `OptionSet` type itself. The `SetAlgebra` protocol is specifically designed to accommodate both kinds of set.

# Conforming to the SetAlgebra Protocol

When implementing a custom type that conforms to the `SetAlgebra` protocol, you must implement the required initializers and methods. For the inherited methods to work properly, conforming types must meet the following axioms. Assume that `S` is a custom type that conforms to the `SetAlgebra` protocol, `x` and `y` are instances of `S`, and `e` is of type `S.Element`—the type that the set holds.

- `S() == []`

- `x.intersection(x) == x`

- `x.intersection([]) == []`

- `x.union(x) == x`

- `x.union([]) == x`

- `x.contains(e)` implies `x.union(y).contains(e)`

- `x.union(y).contains(e)` implies `x.contains(e) || y.contains(e)`

- `x.contains(e) && y.contains(e)` if and only if `x.intersection(y).contains(e)`

- `x.isSubset(of: y)` implies `x.union(y) == y`

- `x.isSuperset(of: y)` implies `x.union(y) == x`

- `x.isSubset(of: y)` if and only if `y.isSuperset(of: x)`

- `x.isStrictSuperset(of: y)` if and only if `x.isSuperset(of: y) && x != y`

- `x.isStrictSubset(of: y)` if and only if `x.isSubset(of: y) && x != y`

## Topics

### Creating a Set

init()

Creates an empty set.

**Required** Default implementation provided.

### Testing for Membership

func contains(Self.Element) -> Bool

Returns a Boolean value that indicates whether the given element exists in the set.

**Required** Default implementation provided.

associatedtype Element

A type for which the conforming type provides a containment test.

**Required**

### Adding and Removing Elements

func insert(Self.Element) -> (inserted: Bool, memberAfterInsert: Self.Element)

Inserts the given element in the set if it is not already present.

**Required** Default implementation provided.

func update(with: Self.Element) -> Self.Element?

Inserts the given element into the set unconditionally.

**Required** Default implementation provided.

func remove(Self.Element) -> Self.Element?

Removes the given element and any elements subsumed by the given element.

**Required** Default implementation provided.

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

func formSymmetricDifference(Self)

Removes the elements of the set that are also in the given set and adds the members of the given set that are not already in the set.

**Required** Default implementation provided.

### Comparing Sets

func isStrictSubset(of: Self) -> Bool

Returns a Boolean value that indicates whether this set is a strict subset of the given set.

func isStrictSuperset(of: Self) -> Bool

Returns a Boolean value that indicates whether this set is a strict superset of the given set.

### Initializers

init&lt;S>(S)

Creates a new set from a finite sequence of items.

**Required** Default implementation provided.

### Instance Properties

var isEmpty: Bool

A Boolean value that indicates whether the set has no elements.

**Required** Default implementation provided.

### Instance Methods

func isDisjoint(with: Self) -> Bool

Returns a Boolean value that indicates whether the set has no members in common with the given set.

**Required** Default implementation provided.

func isSubset(of: Self) -> Bool

Returns a Boolean value that indicates whether the set is a subset of another set.

**Required** Default implementation provided.

func isSuperset(of: Self) -> Bool

Returns a Boolean value that indicates whether the set is a superset of the given set.

**Required** Default implementation provided.

func subtract(Self)

Removes the elements of the given set from this set.

**Required** Default implementation provided.

func subtracting(Self) -> Self

Returns a new set containing the elements of this set that do not occur in the given set.

**Required** Default implementation provided.

## Relationships

### Inherits From

- Equatable
- ExpressibleByArrayLiteral

### Inherited By

- OptionSet

### Conforming Types

- Set

  Conforms when `Element` conforms to `Hashable`.

