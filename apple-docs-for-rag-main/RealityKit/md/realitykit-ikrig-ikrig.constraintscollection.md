

- RealityKit
- IKRig
-  IKRig.ConstraintsCollection 

Structure

# IKRig.ConstraintsCollection

Ordered dictionary-like container.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct ConstraintsCollection
```

## Overview

Supports subscripting by index, element’s identifier or element’s name.

## Topics

### Structures

struct Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

### Initializers

init([IKRig.ConstraintsCollection.Element])

Creates a collection with the provided constraints.

init(arrayLiteral: IKRig.ConstraintsCollection.Element...)

Creates an instance initialized with the given elements.

### Instance Properties

var count: Int

The number of elements in the collection.

var endIndex: IKRig.ConstraintsCollection.Index

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

var isEmpty: Bool

A Boolean value indicating whether the collection is empty.

var startIndex: IKRig.ConstraintsCollection.Index

The position of the first element in a nonempty collection.

### Instance Methods

func contains(IKRig.ConstraintsCollection.Element.ID) -> Bool

Returns a Boolean value that indicates whether the collection contains an element with a specific identifier.

func index(after: IKRig.ConstraintsCollection.Index) -> IKRig.ConstraintsCollection.Index

Returns the position immediately after the given index.

func makeIterator() -> IKRig.ConstraintsCollection.Iterator

Returns an iterator over the elements of the collection.

func set(IKRig.ConstraintsCollection.Element) -> IKRig.ConstraintsCollection.Element?

Updates the element with identifier matching the provided value’s identifier.

### Subscripts

subscript(String) -> IKRig.ConstraintsCollection.Element?

Accesses the element with the specified name.

subscript(IKRig.ConstraintsCollection.Element.ID) -> IKRig.ConstraintsCollection.Element?

Accesses the element with the specified identifier.

subscript(IKRig.ConstraintsCollection.Index) -> IKRig.ConstraintsCollection.Element

Accesses the element at the specified position.

### Type Aliases

typealias ArrayLiteralElement

The type of the elements of an array literal.

typealias Element

A type representing the sequence’s elements.

typealias Index

A type that represents a position in the collection.

typealias Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

typealias SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

### Default Implementations

Collection Implementations

Sequence Implementations

## Relationships

### Conforms To

- Collection
- ExpressibleByArrayLiteral
- Sequence

## See Also

### Inverse kinematics rigs

struct IKRig

A full body inverse kinematics rig definition for a single skeleton.

struct Joint

A definition of a rig joint and its IK solver settings.

struct JointCollection

Ordered dictionary-like container with a fixed size.

struct Constraint

A definition of a rig constraint.

