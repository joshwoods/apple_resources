

- Foundation
-  IndexSet 

Structure

# IndexSet

A collection of unique integer values that represent the indexes of elements in another collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct IndexSet
```

## Overview

The range of valid integer values is `0...Int.max-1`. Anything outside this range is an error.

## Topics

### Creating an Index Set

init()

Initializes an empty index set.

init(integer: IndexSet.Element)

Initializes an index set with a single integer.

init(integersIn: Range&lt;IndexSet.Element>)

Initializes an index set with a range of integers.

### Counting Items in a Set

func count(in: Range&lt;IndexSet.Element>) -> Int

Returns the count of integers in `self` that intersect `range`.

### Combining Index Sets

func formIntersection(IndexSet)

Intersects the `IndexSet` with `other`.

func formSymmetricDifference(IndexSet)

Exclusive or the `IndexSet` with `other`.

func formUnion(IndexSet)

Union the `IndexSet` with `other`.

func intersection(IndexSet) -> IndexSet

Intersects the `IndexSet` with `other`.

func symmetricDifference(IndexSet) -> IndexSet

Exclusive or the `IndexSet` with `other`.

func union(IndexSet) -> IndexSet

Union the `IndexSet` with `other`.

### Inserting Elements

func insert(IndexSet.Element) -> (inserted: Bool, memberAfterInsert: IndexSet.Element)

Insert an integer into the `IndexSet`.

func insert(integersIn: Range&lt;IndexSet.Element>)

Insert a range of integers into the `IndexSet`.

func update(with: IndexSet.Element) -> IndexSet.Element?

Insert an integer into the `IndexSet`.

### Removing Elements

func remove(IndexSet.Element) -> IndexSet.Element?

Remove an integer from the `IndexSet`.

func remove(integersIn: Range&lt;IndexSet.Element>)

Remove a range of integers from the `IndexSet`.

func remove(integersIn: ClosedRange&lt;IndexSet.Element>)

Remove a range of integers from the `IndexSet`.

func removeAll()

Remove all values from the `IndexSet`.

### Testing Set Membership

func contains(IndexSet.Element) -> Bool

Returns `true` if `self` contains `integer`.

func contains(integersIn: IndexSet) -> Bool

Returns `true` if `self` contains all of the integers in `indexSet`.

func contains(integersIn: Range&lt;IndexSet.Element>) -> Bool

Returns `true` if `self` contains all of the integers in `range`.

func intersects(integersIn: Range&lt;IndexSet.Element>) -> Bool

Returns `true` if `self` intersects any of the integers in `range`.

### Manipulating Indexes

func indexRange(in: Range&lt;IndexSet.Element>) -> Range&lt;IndexSet.Index>

Return a `Range` which can be used to subscript the index set.

### Finding Elements

func integerLessThanOrEqualTo(IndexSet.Element) -> IndexSet.Element?

Returns an integer contained in `self` which is less than or equal to `integer`, or `nil` if a result could not be found.

func integerGreaterThan(IndexSet.Element) -> IndexSet.Element?

Returns an integer contained in `self` which is greater than `integer`, or `nil` if a result could not be found.

func integerGreaterThanOrEqualTo(IndexSet.Element) -> IndexSet.Element?

Returns an integer contained in `self` which is greater than or equal to `integer`, or `nil` if a result could not be found.

func integerLessThan(IndexSet.Element) -> IndexSet.Element?

Returns an integer contained in `self` which is less than `integer`, or `nil` if a result could not be found.

### Selecting Elements

func filteredIndexSet(in: Range&lt;IndexSet.Element>, includeInteger: (IndexSet.Element) throws -> Bool) rethrows -> IndexSet

Returns an IndexSet filtered according to the result of `includeInteger`.

func filteredIndexSet(in: ClosedRange&lt;IndexSet.Element>, includeInteger: (IndexSet.Element) throws -> Bool) rethrows -> IndexSet

Returns an IndexSet filtered according to the result of `includeInteger`.

func filteredIndexSet(includeInteger: (IndexSet.Element) throws -> Bool) rethrows -> IndexSet

Returns an IndexSet filtered according to the result of `includeInteger`.

### Shifting Index Groups

func shift(startingAt: IndexSet.Element, by: Int)

For a positive delta, shifts the indexes in \[index, INT_MAX\] to the right, thereby inserting an “empty space” \[index, delta\], for a negative delta, shifts the indexes in \[index, INT_MAX\] to the left, thereby deleting the indexes in the range \[index - delta, delta\].

### Getting a Range-Based View

func rangeView(of: Range&lt;IndexSet.Element>) -> IndexSet.RangeView

Returns a `Range`-based view of `self`.

var rangeView: IndexSet.RangeView

Returns a `Range`-based view of the entire contents of `self`.

struct RangeView

A view of the contents of an IndexSet, organized by range.

### Using Reference Types

class NSIndexSet

An immutable collection of unique integer values that represent indexes in another collection.

class NSMutableIndexSet

A mutable collection of unique integer values that represent indexes in another collection.

### Structures

struct Index

The mechanism for accessing the integers stored in an IndexSet.

### Initializers

init&lt;R>(integersIn: R)

init?(integersIn: RangeSet&lt;Int>)

### Instance Properties

var count: Int

var first: IndexSet.Element?

The first integer in `self`, or nil if `self` is empty.

var isEmpty: Bool

var last: IndexSet.Element?

The last integer in `self`, or nil if `self` is empty.

### Instance Methods

func contains&lt;R>(integersIn: R) -> Bool

func count&lt;R>(in: R) -> Int

func indexRange&lt;R>(in: R) -> Range&lt;IndexSet.Index>

func insert&lt;R>(integersIn: R)

func intersects&lt;R>(integersIn: R) -> Bool

func rangeView&lt;R>(of: R) -> IndexSet.RangeView

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- ExpressibleByArrayLiteral
- Hashable
- ReferenceConvertible
- Sendable
- Sequence
- SetAlgebra

## See Also

### Indexes

struct IndexPath

A list of indexes that together represent the path to a specific location in a tree of nested arrays.

