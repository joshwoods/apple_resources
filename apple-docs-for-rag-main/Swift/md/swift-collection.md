

- Swift
-  Collection 

Protocol

# Collection

A sequence whose elements can be traversed multiple times, nondestructively, and accessed by an indexed subscript.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol Collection : Sequence
```

## Overview

Collections are used extensively throughout the standard library. When you use arrays, dictionaries, and other collections, you benefit from the operations that the `Collection` protocol declares and implements. In addition to the operations that collections inherit from the `Sequence` protocol, you gain access to methods that depend on accessing an element at a specific position in a collection.

For example, if you want to print only the first word in a string, you can search for the index of the first space, and then create a substring up to that position.

```
let text = "Buffalo buffalo buffalo buffalo."
if let firstSpace = text.firstIndex(of: " ") {
    print(text[..

The `firstSpace` constant is an index into the `text` string—the position of the first space in the string. You can store indices in variables, and pass them to collection algorithms or use them later to access the corresponding element. In the example above, `firstSpace` is used to extract the prefix that contains elements up to that index.

# Accessing Individual Elements

You can access an element of a collection through its subscript by using any valid index except the collection’s `endIndex` property. This property is a “past the end” index that does not correspond with any element of the collection.

Here’s an example of accessing the first character in a string through its subscript:

```
let firstChar = text[text.startIndex]
print(firstChar)
// Prints "B"
```

The `Collection` protocol declares and provides default implementations for many operations that depend on elements being accessible by their subscript. For example, you can also access the first character of `text` using the `first` property, which has the value of the first element of the collection, or `nil` if the collection is empty.

```
print(text.first)
// Prints "Optional("B")"
```

You can pass only valid indices to collection operations. You can find a complete set of a collection’s valid indices by starting with the collection’s `startIndex` property and finding every successor up to, and including, the `endIndex` property. All other values of the `Index` type, such as the `startIndex` property of a different collection, are invalid indices for this collection.

Saved indices may become invalid as a result of mutating operations. For more information about index invalidation in mutable collections, see the reference for the `MutableCollection` and `RangeReplaceableCollection` protocols, as well as for the specific type you’re using.

# Accessing Slices of a Collection

You can access a slice of a collection through its ranged subscript or by calling methods like `prefix(while:)` or `suffix(_:)`. A slice of a collection can contain zero or more of the original collection’s elements and shares the original collection’s semantics.

The following example creates a `firstWord` constant by using the `prefix(while:)` method to get a slice of the `text` string.

```
let firstWord = text.prefix(while: { $0 != " " })
print(firstWord)
// Prints "Buffalo"
```

You can retrieve the same slice using the string’s ranged subscript, which takes a range expression.

```
if let firstSpace = text.firstIndex(of: " ") {
    print(text[..

The retrieved slice of `text` is equivalent in each of these cases.

## Slices Share Indices

A collection and its slices share the same indices. An element of a collection is located under the same index in a slice as in the base collection, as long as neither the collection nor the slice has been mutated since the slice was created.

For example, suppose you have an array holding the number of absences from each class during a session.

```
var absences = [0, 2, 0, 4, 0, 3, 1, 0]
```

You’re tasked with finding the day with the most absences in the second half of the session. To find the index of the day in question, follow these steps:

1.  Create a slice of the `absences` array that holds the second half of the days.

2.  Use the `max(by:)` method to determine the index of the day with the most absences.

3.  Print the result using the index found in step 2 on the original `absences` array.

Here’s an implementation of those steps:

```
let secondHalf = absences.suffix(absences.count / 2)
if let i = secondHalf.indices.max(by: { secondHalf[$0] 

## Slices Inherit Collection Semantics

A slice inherits the value or reference semantics of its base collection. That is, when working with a slice of a mutable collection that has value semantics, such as an array, mutating the original collection triggers a copy of that collection and does not affect the contents of the slice.

For example, if you update the last element of the `absences` array from `0` to `2`, the `secondHalf` slice is unchanged.

```
absences[7] = 2
print(absences)
// Prints "[0, 2, 0, 4, 0, 3, 1, 2]"
print(secondHalf)
// Prints "[0, 3, 1, 0]"
```

# Traversing a Collection

Although a sequence can be consumed as it is traversed, a collection is guaranteed to be *multipass*: Any element can be repeatedly accessed by saving its index. Moreover, a collection’s indices form a finite range of the positions of the collection’s elements. The fact that all collections are finite guarantees the safety of many sequence operations, such as using the `contains(_:)` method to test whether a collection includes an element.

Iterating over the elements of a collection by their positions yields the same elements in the same order as iterating over that collection using its iterator. This example demonstrates that the `characters` view of a string returns the same characters in the same order whether the view’s indices or the view itself is being iterated.

```
let word = "Swift"
for character in word {
    print(character)
}
// Prints "S"
// Prints "w"
// Prints "i"
// Prints "f"
// Prints "t"

for i in word.indices {
    print(word[i])
}
// Prints "S"
// Prints "w"
// Prints "i"
// Prints "f"
// Prints "t"
```

# Conforming to the Collection Protocol

If you create a custom sequence that can provide repeated access to its elements, make sure that its type conforms to the `Collection` protocol in order to give a more useful and more efficient interface for sequence and collection operations. To add `Collection` conformance to your type, you must declare at least the following requirements:

- The `startIndex` and `endIndex` properties

- A subscript that provides at least read-only access to your type’s elements

- The `index(after:)` method for advancing an index into your collection

# Expected Performance

Types that conform to `Collection` are expected to provide the `startIndex` and `endIndex` properties and subscript access to elements as O(1) operations. Types that are not able to guarantee this performance must document the departure, because many collection operations depend on O(1) subscripting performance for their own performance guarantees.

The performance of some collection operations depends on the type of index that the collection provides. For example, a random-access collection, which can measure the distance between two indices in O(1) time, can calculate its `count` property in O(1) time. Conversely, because a forward or bidirectional collection must traverse the entire collection to count the number of contained elements, accessing its `count` property is an O(*n*) operation.

## Topics

### Accessing a Collection’s Elements

subscript(Self.Index) -> Self.Element

Accesses the element at the specified position.

**Required** Default implementations provided.

### Selecting and Excluding Elements

func popFirst() -> Self.Element?

Removes and returns the first element of the collection.

func removeFirst() -> Self.Element

Removes and returns the first element of the collection.

func removeFirst(Int)

Removes the specified number of elements from the beginning of the collection.

### Manipulating Indices

var startIndex: Self.Index

The position of the first element in a nonempty collection.

**Required**

var endIndex: Self.Index

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

**Required**

var indices: Self.Indices

The indices that are valid for subscripting the collection, in ascending order.

**Required** Default implementations provided.

func index(after: Self.Index) -> Self.Index

Returns the position immediately after the given index.

**Required** Default implementation provided.

func formIndex(inout Self.Index, offsetBy: Int)

Offsets the given index by the specified distance.

func formIndex(inout Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Bool

Offsets the given index by the specified distance, or so that it equals the given limiting index.

### Iterating Over a Collection’s Elements

func makeIterator() -> Self.Iterator

Returns an iterator over the elements of the collection.

**Required** Default implementation provided.

### Splitting and Joining Elements

func split(separator: Self.Element, maxSplits: Int, omittingEmptySubsequences: Bool) -> [Self.SubSequence]

Returns the longest possible subsequences of the collection, in order, around elements equal to the given element.

func split&lt;C>(separator: C, maxSplits: Int, omittingEmptySubsequences: Bool) -> [Self.SubSequence]

Returns the longest possible subsequences of the collection, in order, around elements equal to the given separator.

func split(maxSplits: Int, omittingEmptySubsequences: Bool, whereSeparator: (Self.Element) throws -> Bool) rethrows -> [Self.SubSequence]

Returns the longest possible subsequences of the collection, in order, that don’t contain elements satisfying the given predicate.

### Related Collection Types

struct DiscontiguousSlice

A collection wrapper that provides access to the elements of a collection, indexed by a set of indices.

### Associated Types

associatedtype Element

A type representing the sequence’s elements.

**Required**

associatedtype Index : Comparable

A type that represents a position in the collection.

**Required**

associatedtype Indices : Collection = DefaultIndices&lt;Self>

A type that represents the indices that are valid for subscripting the collection, in ascending order.

**Required**

associatedtype Iterator = IndexingIterator&lt;Self>

A type that provides the collection’s iteration interface and encapsulates its iteration state.

**Required**

associatedtype SubSequence : Collection = Slice&lt;Self>

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

**Required**

### Instance Properties

var count: Int

The number of elements in the collection.

**Required** Default implementation provided.

var first: Self.Element?

The first element of the collection.

var isEmpty: Bool

A Boolean value indicating whether the collection is empty.

**Required** Default implementation provided.

### Instance Methods

func contains&lt;C>(C) -> Bool

Returns a Boolean value indicating whether the collection contains the given sequence.

func distance(from: Self.Index, to: Self.Index) -> Int

Returns the distance between two indices.

**Required** Default implementations provided.

func drop(while: (Self.Element) throws -> Bool) rethrows -> Self.SubSequence

Returns a subsequence by skipping elements while `predicate` returns `true` and returning the remaining elements.

func dropFirst(Int) -> Self.SubSequence

Returns a subsequence containing all but the given number of initial elements.

func dropLast(Int) -> Self.SubSequence

Returns a subsequence containing all but the specified number of final elements.

func firstIndex(of: Self.Element) -> Self.Index?

Returns the first index where the specified value appears in the collection.

func firstIndex(where: (Self.Element) throws -> Bool) rethrows -> Self.Index?

Returns the first index in which an element of the collection satisfies the given predicate.

func firstRange&lt;C>(of: C) -> Range&lt;Self.Index>?

Finds and returns the range of the first occurrence of a given collection within this collection.

func flatMap((Self.Element) throws -> String?) rethrows -> [String]

func formIndex&lt;T>(inout Self.Index, offsetBy: T)

func formIndex&lt;T>(inout Self.Index, offsetBy: T, limitedBy: Self.Index) -> Bool

func formIndex(after: inout Self.Index)

Replaces the given index with its successor.

**Required** Default implementation provided.

func index(Self.Index, offsetBy: Int) -> Self.Index

Returns an index that is the specified distance from the given index.

**Required** Default implementations provided.

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

**Required** Default implementations provided.

func index(of: Self.Element) -> Self.Index?

Returns the first index where the specified value appears in the collection.

func indices(of: Self.Element) -> RangeSet&lt;Self.Index>

Returns the indices of all the elements that are equal to the given element.

func indices(where: (Self.Element) throws -> Bool) rethrows -> RangeSet&lt;Self.Index>

Returns the indices of all the elements that match the given predicate.

func map&lt;T, E>((Self.Element) throws(E) -> T) throws(E) -> [T]

Returns an array containing the results of mapping the given closure over the sequence’s elements.

func prefix(Int) -> Self.SubSequence

Returns a subsequence, up to the specified maximum length, containing the initial elements of the collection.

func prefix(through: Self.Index) -> Self.SubSequence

Returns a subsequence from the start of the collection through the specified position.

func prefix(upTo: Self.Index) -> Self.SubSequence

Returns a subsequence from the start of the collection up to, but not including, the specified position.

func prefix(while: (Self.Element) throws -> Bool) rethrows -> Self.SubSequence

Returns a subsequence containing the initial elements until `predicate` returns `false` and skipping the remaining elements.

func randomElement() -> Self.Element?

Returns a random element of the collection.

func randomElement&lt;T>(using: inout T) -> Self.Element?

Returns a random element of the collection, using the given generator as a source for randomness.

func ranges&lt;C>(of: C) -> [Range&lt;Self.Index>]

Finds and returns the ranges of the all occurrences of a given sequence within the collection.

func removingSubranges(RangeSet&lt;Self.Index>) -> DiscontiguousSlice&lt;Self>

Returns a collection of the elements in this collection that are not represented by the given range set.

func suffix(Int) -> Self.SubSequence

Returns a subsequence, up to the given maximum length, containing the final elements of the collection.

func suffix(from: Self.Index) -> Self.SubSequence

Returns a subsequence from the specified position to the end of the collection.

func trimPrefix&lt;Prefix>(Prefix)

Removes `prefix` from the start of the collection.

func trimPrefix(while: (Self.Element) throws -> Bool) throws

func trimmingPrefix&lt;Prefix>(Prefix) -> Self.SubSequence

Returns a new collection of the same type by removing `prefix` from the start of the collection.

func trimmingPrefix(while: (Self.Element) throws -> Bool) rethrows -> Self.SubSequence

### Subscripts

subscript(Range&lt;Self.Index>) -> Self.SubSequence

Accesses a contiguous subrange of the collection’s elements.

**Required** Default implementations provided.

### Type Aliases

typealias IndexDistanceDeprecated

## Relationships

### Inherits From

- Sequence

### Inherited By

- BidirectionalCollection
- LazyCollectionProtocol
- MutableCollection
- RandomAccessCollection
- RangeReplaceableCollection
- StringProtocol

### Conforming Types

- AnyBidirectionalCollection

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- AnyCollection

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

- CollectionDifference

  Conforms when `ChangeElement` conforms to `Copyable` and `Escapable`.

- CollectionOfOne

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ContiguousArray

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- DefaultIndices

  Conforms when `Elements` conforms to `RandomAccessCollection`.

- Dictionary

  Conforms when `Key` conforms to `Hashable`, `Value` conforms to `Copyable`, and `Value` conforms to `Escapable`.

- Dictionary.Keys

  Conforms when `Key` conforms to `Hashable`.

- Dictionary.Values

  Conforms when `Key` conforms to `Hashable`.

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

  Conforms when `Base` conforms to `Collection`.

- LazyFilterSequence

  Conforms when `Base` conforms to `Collection`.

- LazyMapSequence

  Conforms when `Base` conforms to `RandomAccessCollection`, `Element` conforms to `Copyable`, and `Element` conforms to `Escapable`.

- LazyPrefixWhileSequence

  Conforms when `Base` conforms to `Collection`.

- LazySequence

  Conforms when `Base` conforms to `BidirectionalCollection`.

- Range

  Conforms when `Bound` conforms to `Strideable` and `Bound.Stride` conforms to `SignedInteger`.

- RangeSet.Ranges

  Conforms when `Bound` conforms to `Comparable`.

- Repeated

  Conforms when `Element` conforms to `Copyable` and `Escapable`.

- ReversedCollection

  Conforms when `Base` conforms to `RandomAccessCollection`.

- Set

  Conforms when `Element` conforms to `Hashable`.

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

### First Steps

protocol Sequence

A type that provides sequential, iterated access to its elements.

