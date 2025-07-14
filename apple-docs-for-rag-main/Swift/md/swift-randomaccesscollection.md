

- Swift
-  RandomAccessCollection 

Protocol

# RandomAccessCollection

A collection that supports efficient random-access index traversal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol RandomAccessCollection : BidirectionalCollection where Self.Indices : RandomAccessCollection, Self.SubSequence : RandomAccessCollection
```

## Overview

Random-access collections can move indices any distance and measure the distance between indices in O(1) time. Therefore, the fundamental difference between random-access and bidirectional collections is that operations that depend on index movement or distance measurement offer significantly improved efficiency. For example, a random-access collection’s `count` property is calculated in O(1) instead of requiring iteration of an entire collection.

# Conforming to the RandomAccessCollection Protocol

The `RandomAccessCollection` protocol adds further constraints on the associated `Indices` and `SubSequence` types, but otherwise imposes no additional requirements over the `BidirectionalCollection` protocol. However, in order to meet the complexity guarantees of a random-access collection, either the index for your custom type must conform to the `Strideable` protocol or you must implement the `index(_:offsetBy:)` and `distance(from:to:)` methods with O(1) efficiency.

## Topics

### Associated Types

associatedtype Element

A type representing the sequence’s elements.

**Required**

associatedtype Index

A type that represents a position in the collection.

**Required**

associatedtype Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

**Required**

associatedtype SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

**Required**

### Instance Properties

var endIndex: Self.Index

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

**Required**

var indices: Self.Indices

The indices that are valid for subscripting the collection, in ascending order.

**Required** Default implementation provided.

var startIndex: Self.Index

The position of the first element in a nonempty collection.

**Required**

### Instance Methods

func distance(from: Self.Index, to: Self.Index) -> Int

Returns the distance between two indices.

**Required** Default implementation provided.

func formIndex(after: inout Self.Index)

Replaces the given index with its successor.

**Required**

func formIndex(before: inout Self.Index)

Replaces the given index with its predecessor.

**Required**

func index(Self.Index, offsetBy: Int) -> Self.Index

Returns an index that is the specified distance from the given index.

**Required** Default implementation provided.

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

**Required** Default implementation provided.

func index(after: Self.Index) -> Self.Index

Returns the position immediately after the given index.

**Required** Default implementation provided.

func index(before: Self.Index) -> Self.Index

Returns the position immediately before the given index.

**Required** Default implementation provided.

### Subscripts

subscript(Self.Index) -> Self.Element

Accesses the element at the specified position.

**Required**

subscript(Range&lt;Self.Index>) -> Self.SubSequence

Accesses a contiguous subrange of the collection’s elements.

**Required**

## Relationships

### Inherits From

- BidirectionalCollection
- Collection
- Sequence

### Conforming Types

- AnyRandomAccessCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- AnyRegexOutput
- Array

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ArraySlice

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ClosedRange

  Conforms when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

- CollectionOfOne

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ContiguousArray

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- DefaultIndices

  Conforms when `Elements` conforms to `RandomAccessCollection`.

- EmptyCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- Int.Words
- Int16.Words
- Int32.Words
- Int64.Words
- Int8.Words
- KeyValuePairs

  Conforms when `Key` conforms to `Copyable`, `Key` conforms to `Escapable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- LazyMapSequence

  Conforms when `Base` conforms to `RandomAccessCollection`, `Element` conforms to `Copyable`, and `Element` conforms to `Escapable`.

- LazySequence

  Conforms when `Base` conforms to `RandomAccessCollection`.

- Range

  Conforms when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

- RangeSet.Ranges

  Conforms when `Bound` conforms to `Comparable`.

- Repeated

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ReversedCollection

  Conforms when `Base` conforms to `RandomAccessCollection`.

- Slice

  Conforms when `Base` conforms to `RandomAccessCollection`.

- UInt.Words
- UInt128.Words
- UInt16.Words
- UInt32.Words
- UInt64.Words
- UInt8.Words
- Unicode.Scalar.UTF16View
- Unicode.Scalar.UTF8View
- UnsafeBufferPointer

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- UnsafeMutableBufferPointer

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- UnsafeMutableRawBufferPointer
- UnsafeRawBufferPointer

## See Also

### Collection Traversal

protocol BidirectionalCollection

A collection that supports backward as well as forward traversal.

