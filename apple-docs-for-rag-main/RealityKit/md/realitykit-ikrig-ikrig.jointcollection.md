

- RealityKit
- IKRig
-  IKRig.JointCollection 

Structure

# IKRig.JointCollection

Ordered dictionary-like container with a fixed size.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct JointCollection
```

## Overview

Supports subscripting by index, element’s identifier or element’s name.

## Topics

### Structures

struct Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

### Instance Properties

var count: Int

The number of elements in the collection.

var endIndex: IKRig.JointCollection.Index

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

var isEmpty: Bool

A Boolean value indicating whether the collection is empty.

var startIndex: IKRig.JointCollection.Index

The position of the first element in a nonempty collection.

### Instance Methods

func contains(IKRig.JointCollection.Element.ID) -> Bool

Returns a Boolean value that indicates whether the collection contains an element with a specific identifier.

func forEach(descendantOf: String, inclusive: Bool, update: (inout IKRig.JointCollection.Element) -> Void)

Calls the provided closure on each element in the hierarchy rooted at the named joint.

func index(after: IKRig.JointCollection.Index) -> IKRig.JointCollection.Index

Returns the position immediately after the given index.

func makeIterator() -> IKRig.JointCollection.Iterator

Returns an iterator over the elements of the collection.

func set(IKRig.JointCollection.Element) -> IKRig.JointCollection.Element?

Updates the element with identifier matching the provided value’s identifier.

### Subscripts

subscript(String) -> IKRig.JointCollection.Element?

Accesses the element with the specified name.

subscript(IKRig.JointCollection.Element.ID) -> IKRig.JointCollection.Element?

Accesses the element with the specified identifier.

subscript(IKRig.JointCollection.Index) -> IKRig.JointCollection.Element

Accesses the element at the specified position.

### Type Aliases

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
- Sequence

## See Also

### Inverse kinematics rigs

struct IKRig

A full body inverse kinematics rig definition for a single skeleton.

struct Joint

A definition of a rig joint and its IK solver settings.

struct Constraint

A definition of a rig constraint.

struct ConstraintsCollection

Ordered dictionary-like container.

