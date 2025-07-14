

- Foundation
- IndexSet
-  IndexSet.RangeView 

Structure

# IndexSet.RangeView

A view of the contents of an IndexSet, organized by range.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct RangeView
```

## Overview

For example, if an IndexSet is composed of: `[1..

## Topics

### Counting Indexes

var count: Int

var first: IndexSet.Element?

The first integer in `self`, or nil if `self` is empty.

var isEmpty: Bool

var last: IndexSet.Element?

The last integer in `self`, or nil if `self` is empty.

### Testing for Inclusion in the Range

func contains(IndexSet.Element) -> Bool

Returns `true` if `self` contains `integer`.

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Equatable
- Sendable
- Sequence

## See Also

### Getting a Range-Based View

func rangeView(of: Range&lt;IndexSet.Element>) -> IndexSet.RangeView

Returns a `Range`-based view of `self`.

var rangeView: IndexSet.RangeView

Returns a `Range`-based view of the entire contents of `self`.

