

- RealityKit
- IKComponent
-  IKComponent.JointCollection 

Structure

# IKComponent.JointCollection

Ordered dictionary like container with fixed size.

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

var endIndex: IKComponent.JointCollection.Index

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

var isEmpty: Bool

A Boolean value indicating whether the collection is empty.

var startIndex: IKComponent.JointCollection.Index

The position of the first element in a nonempty collection.

### Instance Methods

func contains(IKComponent.JointCollection.Element.ID) -> Bool

Returns a Boolean value that indicates whether the collection contains an element with a specific identifier.

func index(after: IKComponent.JointCollection.Index) -> IKComponent.JointCollection.Index

Returns the position immediately after the given index.

func makeIterator() -> IKComponent.JointCollection.Iterator

Returns an iterator over the elements of the collection.

func set(IKComponent.JointCollection.Element) -> IKComponent.JointCollection.Element?

Updates the element with identifier matching the new value.

### Subscripts

subscript(IKComponent.JointCollection.Index) -> IKComponent.JointCollection.Element

Accesses the element at the specified position.

subscript(String) -> IKComponent.JointCollection.Element?

Accesses the element with the specified name.

subscript(IKComponent.JointCollection.Element.ID) -> IKComponent.JointCollection.Element?

Accesses the element with the specified identifier.

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

### Inverse kinematics components

struct IKComponent

A component that allows you to procedurally animate a skeletal model using a full body inverse kinematics solver.

class Joint

The update stage object that lets you read and update the current settings of a single joint in an IK solver.

class Solver

The update stage object that lets you read and update the current settings of a single solver instance.

struct SolverCollection

Ordered dictionary like container with fixed size.

class Constraint

The update stage object that lets you read and update the current settings of a single constraint in an IK solver.

struct ConstraintCollection

Ordered dictionary like container with fixed size.

class IKResource

A reference counted immutable resource which contains one or more inverse kinematics solver rigs.

struct IKSolverDefinition

A container describing a solver instance.

typealias ID

A type representing the stable identity of the entity associated with an instance.

