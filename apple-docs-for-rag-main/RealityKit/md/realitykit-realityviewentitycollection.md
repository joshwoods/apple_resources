

- RealityKit
-  RealityViewEntityCollection 

Structure

# RealityViewEntityCollection

A collection of entities in a RealityView.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
struct RealityViewEntityCollection
```

## Overview

This collection is used by entities.

## Topics

### Instance Properties

var count: Int

The number of elements in the collection.

var endIndex: Int

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

var startIndex: Int

The position of the first element in a nonempty collection.

### Instance Methods

func append&lt;S>(contentsOf: S)

Adds the specified sequence of entities to the end of this collection, in order.

func index(after: Int) -> Int

Returns the position immediately after the given index.

func insert&lt;S>(contentsOf: S, beforeIndex: Int)

Adds the specified sequence of entities to this collection in order, directly before the entity at the given index.

func remove(Entity)

Removes the entity from the collection.

func remove(at: Int)

Removes the entity at the given index from this collection.

func removeAll()

Removes all entities from this collection.

func replaceAll&lt;S>(S)

Replaces all entities in this collection with those from the given sequence.

### Subscripts

subscript(Int) -> Entity

Accesses the element at the specified position.

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

EntityCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- Collection
- EntityCollection
- Sequence

## See Also

### SwiftUI scene presentation

struct RealityView

A view that contains RealityKit content.

struct RealityViewContent

The content of a visionOS reality view.

struct RealityViewCameraContent

The content of a reality view that is displayed through a camera.

protocol RealityViewContentProtocol

A protocol representing the content of a reality view.

struct RealityViewDefaultPlaceholder

A view that represents the default placeholder for a RealityView.

protocol EntityCollection

An ordered, mutable collection of entities.

