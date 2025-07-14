

- RealityKit
- Entity
- Entity.ComponentSet
-  Entity.ComponentSet.Indices 

Structure

# Entity.ComponentSet.Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct Indices
```

## Topics

### Instance Properties

var endIndex: Entity.ComponentSet.Indices.Index

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

var indices: Entity.ComponentSet.Indices

The indices that are valid for subscripting the collection, in ascending order.

var startIndex: Entity.ComponentSet.Indices.Index

The position of the first element in a nonempty collection.

### Instance Methods

func distance(from: Entity.ComponentSet.Indices.Index, to: Entity.ComponentSet.Indices.Index) -> Int

Returns the distance between two indices.

func formIndex(after: inout Entity.ComponentSet.Indices.Index)

Replaces the given index with its successor.

func index(after: Entity.ComponentSet.Indices.Index) -> Entity.ComponentSet.Indices.Index

Returns the position immediately after the given index.

### Subscripts

subscript(Entity.ComponentSet.Indices.Index) -> Entity.ComponentSet.Indices.Index

Accesses the element at the specified position.

subscript(Range&lt;Entity.ComponentSet.Indices.Index>) -> Entity.ComponentSet.Indices

Accesses a contiguous subrange of the collection’s elements.

### Type Aliases

typealias Element

A type representing the sequence’s elements.

typealias Index

A type that represents a position in the collection.

typealias Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

typealias Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

typealias SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

### Default Implementations

Collection Implementations

Sequence Implementations

## Relationships

### Conforms To

- Collection
- Sendable
- Sequence

