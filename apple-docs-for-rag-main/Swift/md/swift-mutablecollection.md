

- Swift
-  MutableCollection 

Protocol

# MutableCollection

A collection that supports subscript assignment.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol MutableCollection : Collection where Self.SubSequence : MutableCollection
```

## Overview

Collections that conform to `MutableCollection` gain the ability to change the value of their elements. This example shows how you can modify one of the names in an array of students.

```
var students = ["Ben", "Ivy", "Jordell", "Maxime"]
if let i = students.firstIndex(of: "Maxime") {
    students[i] = "Max"
}
print(students)
// Prints "["Ben", "Ivy", "Jordell", "Max"]"
```

In addition to changing the value of an individual element, you can also change the values of a slice of elements in a mutable collection. For example, you can sort *part* of a mutable collection by calling the mutable `sort()` method on a subscripted subsequence. Here’s an example that sorts the first half of an array of integers:

```
var numbers = [15, 40, 10, 30, 60, 25, 5, 100]
numbers[0..

The `MutableCollection` protocol allows changing the values of a collection’s elements but not the length of the collection itself. For operations that require adding or removing elements, see the `RangeReplaceableCollection` protocol instead.

# Conforming to the MutableCollection Protocol

To add conformance to the `MutableCollection` protocol to your own custom collection, upgrade your type’s subscript to support both read and write access.

A value stored into a subscript of a `MutableCollection` instance must subsequently be accessible at that same position. That is, for a mutable collection instance `a`, index `i`, and value `x`, the two sets of assignments in the following code sample must be equivalent:

```
a[i] = x
let y = a[i]

// Must be equivalent to:
a[i] = x
let y = x
```

## Topics

### Associated Types

associatedtype Element

A type representing the sequence’s elements.

**Required**

associatedtype Index

A type that represents a position in the collection.

**Required**

associatedtype SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

**Required**

### Instance Methods

func move(fromOffsets: IndexSet, toOffset: Int)

Moves all the elements at the specified offsets to the specified destination offset, preserving ordering.

func moveSubranges(RangeSet&lt;Self.Index>, to: Self.Index) -> Range&lt;Self.Index>

Moves the elements in the given subranges to just before the element at the specified index.

func partition(by: (Self.Element) throws -> Bool) rethrows -> Self.Index

Reorders the elements of the collection such that all the elements that match the given predicate are after all the elements that don’t match.

**Required** Default implementations provided.

func removeSubranges(RangeSet&lt;Self.Index>)

Removes the elements at the given indices.

func reverse()

Reverses the elements of the collection in place.

func shuffle()

Shuffles the collection in place.

func shuffle&lt;T>(using: inout T)

Shuffles the collection in place, using the given generator as a source for randomness.

func sort()

Sorts the collection in place.

func sort(by: (Self.Element, Self.Element) throws -> Bool) rethrows

Sorts the collection in place, using the given predicate as the comparison between elements.

func sort&lt;Comparator>(using: Comparator)

Sorts the collection using the given comparator to compare elements.

func sort&lt;S, Comparator>(using: S)

Sorts the collection using the given array of `SortComparator`s to compare elements.

func swapAt(Self.Index, Self.Index)

Exchanges the values at the specified indices of the collection.

**Required** Default implementation provided.

func withContiguousMutableStorageIfAvailable&lt;R>((inout UnsafeMutableBufferPointer&lt;Self.Element>) throws -> R) rethrows -> R?

Executes a closure on the collection’s contiguous storage.

**Required** Default implementation provided.

### Subscripts

subscript(Range&lt;Self.Index>) -> Self.SubSequence

Accesses a contiguous subrange of the collection’s elements.

**Required** Default implementations provided.

subscript(Self.Index) -> Self.Element

Accesses the element at the specified position.

**Required** Default implementations provided.

## Relationships

### Inherits From

- Collection
- Sequence

### Conforming Types

- Array

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ArraySlice

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- CollectionOfOne

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ContiguousArray

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Dictionary.Values

  Conforms when `Key` conforms to `Hashable`.

- EmptyCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Slice

  Conforms when `Base` conforms to `MutableCollection`.

- UnsafeMutableBufferPointer

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- UnsafeMutableRawBufferPointer

## See Also

### Collection Mutability

protocol RangeReplaceableCollection

A collection that supports replacement of an arbitrary subrange of elements with the elements of another collection.

