

- RealityKit
- AnchoringComponent
- AnchoringComponent.Target
-  AnchoringComponent.Target.Classification 

Structure

# AnchoringComponent.Target.Classification

Defines types of real-world surfaces to seek as targets.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+visionOS

``` source
struct Classification
```

## Topics

### Classifying a target

static let wall: AnchoringComponent.Target.Classification

Look for walls.

static let floor: AnchoringComponent.Target.Classification

Look for floors.

static let ceiling: AnchoringComponent.Target.Classification

Look for ceilings.

static let table: AnchoringComponent.Target.Classification

Look for tables.

static let seat: AnchoringComponent.Target.Classification

Look for seats.

static let any: AnchoringComponent.Target.Classification

Look for any kind of surface.

### Creating a target classification instance

init()

Creates an empty option set.

init&lt;S>(S)

Creates a new set from a finite sequence of items.

init(arrayLiteral: Self.Element...)

Creates a set containing the elements of the given array literal.

init(rawValue: UInt64)

Creates a new option set from the given raw value.

### Option set conformance

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

The element type of the option set.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

var isEmpty: Bool

A Boolean value that indicates whether the set has no elements.

let rawValue: UInt64

The corresponding value of the raw type.

func contains(Self) -> Bool

Returns a Boolean value that indicates whether a given element is a member of the option set.

func formIntersection(Self)

Removes all elements of this option set that are not also present in the given set.

func formSymmetricDifference(Self)

Replaces this set with a new set containing all elements contained in either this set or the given set, but not in both.

func formUnion(Self)

Inserts the elements of another set into this option set.

func insert(Self.Element) -> (inserted: Bool, memberAfterInsert: Self.Element)

Adds the given element to the option set if it is not already a member.

func intersection(Self) -> Self

Returns a new option set with only the elements contained in both this set and the given set.

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

func remove(Self.Element) -> Self.Element?

Removes the given element and all elements subsumed by it.

func subtract(Self)

Removes the elements of the given set from this set.

func subtracting(Self) -> Self

Returns a new set containing the elements of this set that do not occur in the given set.

func symmetricDifference(Self) -> Self

Returns a new option set with the elements contained in this set or in the given set, but not in both.

func union(Self) -> Self

Returns a new option set of the elements contained in this set, in the given set, or in both.

func update(with: Self.Element) -> Self.Element?

Inserts the given element into the set.

### Default Implementations

Equatable Implementations

OptionSet Implementations

SetAlgebra Implementations

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

## See Also

### Surface anchor characterization

struct Alignment

Defines the alignment of real-world surfaces to seek as targets.

