

- Swift
-  RangeSet 

Structure

# RangeSet

A set of values of any comparable type, represented by ranges.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct RangeSet where Bound : Comparable
```

## Overview

You can use a range set to efficiently represent a set of `Comparable` values that spans any number of discontiguous ranges. Range sets are commonly used to represent multiple subranges of a collection, by storing ranges of a collection’s index type.

In this example, `negativeSubranges` is a range set representing the locations of all the negative values in `numbers`:

```
var numbers = [10, 12, -5, 14, -3, -9, 15]
let negativeSubranges = numbers.subranges(where: { $0 

## Topics

### Structures

struct Ranges

A collection of the ranges that make up a range set.

### Initializers

init()

Creates an empty range set.

init(Range&lt;Bound>)

Creates a range set containing the given range.

init(IndexSet)

init(some Sequence&lt;Range&lt;Bound>>)

Creates a range set containing the values in the given ranges.

init&lt;S, C>(S, within: C)

Creates a new range set containing ranges that contain only the specified indices in the given collection.

### Instance Properties

var isEmpty: Bool

A Boolean value indicating whether the range set is empty.

var ranges: RangeSet&lt;Bound>.Ranges

A collection of the ranges that make up the range set.

### Instance Methods

func contains(Bound) -> Bool

Returns a Boolean value indicating whether the given value is contained by the ranges in the range set.

func formIntersection(RangeSet&lt;Bound>)

Removes the contents of this range set that aren’t also in the given range set.

func formSymmetricDifference(RangeSet&lt;Bound>)

Removes the contents of this range set that are also in the given set and adds the contents of the given set that are not already in this range set.

func formUnion(RangeSet&lt;Bound>)

Adds the contents of the given range set to this range set.

func insert&lt;C>(Bound, within: C) -> Bool

Inserts a range that contains only the specified index into the range set.

func insert(contentsOf: Range&lt;Bound>)

Inserts the given range into the range set.

func intersection(RangeSet&lt;Bound>) -> RangeSet&lt;Bound>

Returns a new range set containing the contents of both this set and the given set.

func isDisjoint(RangeSet&lt;Bound>) -> Bool

Returns a Boolean value that indicates whether this range set set has no members in common with the given set.

func isStrictSubset(of: RangeSet&lt;Bound>) -> Bool

Returns a Boolean value that indicates whether this range set is a strict subset of the given set.

func isStrictSuperset(of: RangeSet&lt;Bound>) -> Bool

Returns a Boolean value that indicates whether this range set is a strict superset of the given set.

func isSubset(of: RangeSet&lt;Bound>) -> Bool

Returns a Boolean value that indicates whether this range set is a subset of the given set.

func isSuperset(of: RangeSet&lt;Bound>) -> Bool

Returns a Boolean value that indicates whether this range set is a superset of the given set.

func remove&lt;C>(Bound, within: C)

Removes the range that contains only the specified index from the range set.

func remove(contentsOf: Range&lt;Bound>)

Removes the given range from the range set.

func subtract(RangeSet&lt;Bound>)

Removes the contents of the given range set from this range set.

func subtracting(RangeSet&lt;Bound>) -> RangeSet&lt;Bound>

Returns a new set containing the contents of this range set that are not also in the given range set.

func symmetricDifference(RangeSet&lt;Bound>) -> RangeSet&lt;Bound>

Returns a new range set representing the values in this range set or the given range set, but not both.

func union(RangeSet&lt;Bound>) -> RangeSet&lt;Bound>

Returns a new range set containing the contents of both this set and the given set.

### Default Implementations

CustomStringConvertible Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable

  Conforms when `Bound` conforms to `Comparable` and `Hashable`.

- CustomStringConvertible

  Conforms when `Bound` conforms to `Comparable`.

- Equatable

  Conforms when `Bound` conforms to `Comparable` and `Hashable`.

- Hashable

  Conforms when `Bound` conforms to `Comparable` and `Hashable`.

- Sendable

  Conforms when `Bound` conforms to `Comparable` and `Sendable`.

## See Also

### Ranges

static func ..&lt; (Self, Self) -> Range&lt;Self>

Returns a half-open range that contains its lower bound but not its upper bound.

struct Range

A half-open interval from a lower bound up to, but not including, an upper bound.

static func ... (Self, Self) -> ClosedRange&lt;Self>

Returns a closed range that contains both of its bounds.

struct ClosedRange

An interval from a lower bound up to, and including, an upper bound.

