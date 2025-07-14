

- Swift
-  BidirectionalCollection 

Protocol

# BidirectionalCollection

A collection that supports backward as well as forward traversal.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol BidirectionalCollection : Collection where Self.Indices : BidirectionalCollection, Self.SubSequence : BidirectionalCollection
```

## Overview

Bidirectional collections offer traversal backward from any valid index, not including a collection’s `startIndex`. Bidirectional collections can therefore offer additional operations, such as a `last` property that provides efficient access to the last element and a `reversed()` method that presents the elements in reverse order. In addition, bidirectional collections have more efficient implementations of some sequence and collection methods, such as `suffix(_:)`.

# Conforming to the BidirectionalCollection Protocol

To add `BidirectionalProtocol` conformance to your custom types, implement the `index(before:)` method in addition to the requirements of the `Collection` protocol.

Indices that are moved forward and backward in a bidirectional collection move by the same amount in each direction. That is, for any valid index `i` into a bidirectional collection `c`:

- If `i >= c.startIndex && i  c.startIndex && i 

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

var last: Self.Element?

The last element of the collection.

var startIndex: Self.Index

The position of the first element in a nonempty collection.

**Required**

### Instance Methods

func contains(some RegexComponent) -> Bool

Returns a Boolean value indicating whether the collection contains the given regex.

func contains(() -> some RegexComponent) -> Bool

Returns a Boolean value indicating whether this collection contains a match for the regex, where the regex is created by the given closure.

func difference&lt;C>(from: C) -> CollectionDifference&lt;Self.Element>

Returns the difference needed to produce this collection’s ordered elements from the given collection.

func difference&lt;C>(from: C, by: (C.Element, Self.Element) -> Bool) -> CollectionDifference&lt;Self.Element>

Returns the difference needed to produce this collection’s ordered elements from the given collection, using the given predicate as an equivalence test.

func distance(from: Self.Index, to: Self.Index) -> Int

Returns the distance between two indices.

**Required** Default implementations provided.

func dropLast(Int) -> Self.SubSequence

Returns a subsequence containing all but the specified number of final elements.

func firstMatch&lt;Output>(of: () -> some RegexComponent) -> Regex&lt;Output>.Match?

Returns the first match for the regex within this collection, where the regex is created by the given closure.

func firstMatch&lt;Output>(of: some RegexComponent) -> Regex&lt;Output>.Match?

Returns the first match of the specified regex within the collection.

func firstRange(of: some RegexComponent) -> Range&lt;Self.Index>?

Finds and returns the range of the first occurrence of a given regex within the collection.

func firstRange(of: () -> some RegexComponent) -> Range&lt;Self.Index>?

Returns the range of the first match for the regex within this collection, where the regex is created by the given closure.

func firstRange&lt;C>(of: C) -> Range&lt;Self.Index>?

Finds and returns the range of the first occurrence of a given collection within this collection.

func formIndex(after: inout Self.Index)

Replaces the given index with its successor.

**Required**

func formIndex(before: inout Self.Index)

Replaces the given index with its predecessor.

**Required** Default implementation provided.

func index(Self.Index, offsetBy: Int) -> Self.Index

Returns an index that is the specified distance from the given index.

**Required** Default implementations provided.

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

**Required** Default implementations provided.

func index(after: Self.Index) -> Self.Index

Returns the position immediately after the given index.

**Required** Default implementation provided.

func index(before: Self.Index) -> Self.Index

Returns the position immediately before the given index.

**Required** Default implementation provided.

func joined(separator: String) -> String

Returns a new string by concatenating the elements of the sequence, adding the given separator between each element.

func last(where: (Self.Element) throws -> Bool) rethrows -> Self.Element?

Returns the last element of the sequence that satisfies the given predicate.

func lastIndex(of: Self.Element) -> Self.Index?

Returns the last index where the specified value appears in the collection.

func lastIndex(where: (Self.Element) throws -> Bool) rethrows -> Self.Index?

Returns the index of the last element in the collection that matches the given predicate.

func matches&lt;Output>(of: () -> some RegexComponent) -> [Regex&lt;Output>.Match]

Returns a collection containing all non-overlapping matches of the regex, created by the given closure.

func matches&lt;Output>(of: some RegexComponent) -> [Regex&lt;Output>.Match]

Returns a collection containing all matches of the specified regex.

func popLast() -> Self.Element?

Removes and returns the last element of the collection.

func prefixMatch&lt;Output>(of: () -> some RegexComponent) -> Regex&lt;Output>.Match?

Matches part of the regex, starting at the beginning, where the regex is created by the given closure.

func prefixMatch&lt;R>(of: R) -> Regex&lt;R.RegexOutput>.Match?

Returns a match if this string is matched by the given regex at its start.

func ranges(of: some RegexComponent) -> [Range&lt;Self.Index>]

Finds and returns the ranges of the all occurrences of a given sequence within the collection.

func ranges(of: () -> some RegexComponent) -> [Range&lt;Self.Index>]

Returns the ranges of the all non-overlapping matches for the regex within this collection, where the regex is created by the given closure.

func removeLast() -> Self.Element

Removes and returns the last element of the collection.

func removeLast(Int)

Removes the given number of elements from the end of the collection.

func reversed() -> ReversedCollection&lt;Self>

Returns a view presenting the elements of the collection in reverse order.

func split(maxSplits: Int, omittingEmptySubsequences: Bool, separator: () -> some RegexComponent) -> [Self.SubSequence]

Returns the longest possible subsequences of the collection, in order, around subsequence that match the regex created by the given closure.

func split(separator: some RegexComponent, maxSplits: Int, omittingEmptySubsequences: Bool) -> [Self.SubSequence]

Returns the longest possible subsequences of the collection, in order, around elements equal to the given separator.

func starts(with: some RegexComponent) -> Bool

Returns a Boolean value indicating whether the initial elements of the sequence are the same as the elements in the specified regex.

func starts(with: () -> some RegexComponent) -> Bool

Returns a Boolean value indicating whether the initial elements of this collection are a match for the regex created by the given closure.

func suffix(Int) -> Self.SubSequence

Returns a subsequence, up to the given maximum length, containing the final elements of the collection.

func trimmingPrefix(some RegexComponent) -> Self.SubSequence

Returns a new collection of the same type by removing the initial elements that matches the given regex.

func trimmingPrefix(() -> some RegexComponent) -> Self.SubSequence

Returns a subsequence of this collection by removing the elements matching the regex from the start, where the regex is created by the given closure.

func wholeMatch&lt;Output>(of: () -> some RegexComponent) -> Regex&lt;Output>.Match?

Matches a regex in its entirety, where the regex is created by the given closure.

func wholeMatch&lt;R>(of: R) -> Regex&lt;R.RegexOutput>.Match?

Returns a match if this string is matched by the given regex in its entirety.

### Subscripts

subscript(Self.Index) -> Self.Element

Accesses the element at the specified position.

**Required**

subscript(Range&lt;Self.Index>) -> Self.SubSequence

Accesses a contiguous subrange of the collection’s elements.

**Required**

## Relationships

### Inherits From

- Collection
- Sequence

### Inherited By

- RandomAccessCollection
- StringProtocol

### Conforming Types

- AnyBidirectionalCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

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

  Conforms when `Elements` conforms to `BidirectionalCollection`.

- DiscontiguousSlice

  Conforms when `Base` conforms to `BidirectionalCollection`.

- EmptyCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- FlattenSequence

  Conforms when `Base` conforms to `BidirectionalCollection` and `Base.Element` conforms to `BidirectionalCollection`.

- Int.Words
- Int16.Words
- Int32.Words
- Int64.Words
- Int8.Words
- KeyValuePairs

  Conforms when `Key` conforms to `Copyable`, `Key` conforms to `Escapable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- LazyDropWhileSequence

  Conforms when `Base` conforms to `BidirectionalCollection`.

- LazyFilterSequence

  Conforms when `Base` conforms to `BidirectionalCollection`.

- LazyMapSequence

  Conforms when `Base` conforms to `BidirectionalCollection`, `Element` conforms to `Copyable`, and `Element` conforms to `Escapable`.

- LazyPrefixWhileSequence

  Conforms when `Base` conforms to `BidirectionalCollection`.

- LazySequence

  Conforms when `Base` conforms to `BidirectionalCollection`.

- Range

  Conforms when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

- RangeSet.Ranges

  Conforms when `Bound` conforms to `Comparable`.

- Repeated

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ReversedCollection

  Conforms when `Base` conforms to `BidirectionalCollection`.

- Slice

  Conforms when `Base` conforms to `BidirectionalCollection`.

- String
- String.UTF16View
- String.UTF8View
- String.UnicodeScalarView
- Substring
- Substring.UTF16View
- Substring.UTF8View
- Substring.UnicodeScalarView
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

protocol RandomAccessCollection

A collection that supports efficient random-access index traversal.

